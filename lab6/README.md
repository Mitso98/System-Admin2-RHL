<!-- Output copied to clipboard! -->

<!-- You have some errors, warnings, or alerts. If you are using reckless mode, turn it off to see inline alerts.
* ERRORs: 0
* WARNINGs: 0
* ALERTS: 34 -->

**Lab 6 :**

1. **Find out what device node the /boot partition is **

   **df -h /boot**

![alt_text](images/image1.png "image_tooltip")

![alt_text](images/image2.png "image_tooltip")

1. **Estimate the size in bytes of a level-zero dump for /boot**

**=> sudo dump S /boot **

2. **Back up the data of /boot to a dump file in /var/tmp/dumpfile => Back up the data of /boot to a dump file in /var/tmp/dumpfile**
3. ** Look in the /etc/dumpdates file and see how the dump command recorded the timestamp of the full backup**

   **=> vi /etc/dumpdates**

4. **Use the restore command to view the contents of the dump file**

   **=> restore -if /var/tmp/dumpfile**

5. **Use restore command in the interactive mode to extract /grub/splash.xpm.gz and /grub/grub.conf**

** => restore -if /var/tmp/dumpfile /grub/splash.xpm.gz /grub/grub.conf**

    ** **

6. **Use the fdisk command to create 2 Linux LVM (0x8e) partitions using "unpartitioned" space on your hard disk. These partitions should all be the same size; to speed up the lab, do not make them larger than 300 MB each. Make sure to write the changes to disk by using the w command to exit the fdisk utility. Run the partprobe command after exiting the fdisk utility.**

** => sudo dump -u0 -f /var/tmp/dumpfile /boot **

    **8. Initialize your Linux LVM partitions as physical volumes with the pvcreate**


    **command. You can use the pvdisplay command to verify that the partitions have**


    **been initialized as physical volumes.**


    ** **

![alt_text](images/image3.png "image_tooltip")

![alt_text](images/image4.png "image_tooltip")

    **9. Using only one of your physical volumes, create a volume group called test0. Use**


    **the vgdisplay command to verify that the volume group was created.**

![alt_text](images/image5.png "image_tooltip")

![alt_text](images/image6.png "image_tooltip")

    **10. Create a small logical volume (LV) called data that uses about 30 percent of the**


    **available space of the test0 volume group. Look for VG Size and Free PE/Size in**


    **the output of the vgdisplay command to assist you with this. Use the lvdisplay**


    **command to verify your work.**

![alt_text](images/image7.png "image_tooltip")

![alt_text](images/image8.png "image_tooltip")

    **11. Create an ext2 filesystem on your new LV.**

![alt_text](images/image9.png "image_tooltip")

    **12. Make a new directory called /data and then mount the new LV under the /data**


    **directory. Create a "large file" in this volume.**

![alt_text](images/image10.png "image_tooltip")

![alt_text](images/image11.png "image_tooltip")

![alt_text](images/image12.png "image_tooltip")

    **Edit in fstap file**

![alt_text](images/image13.png "image_tooltip")

![alt_text](images/image14.png "image_tooltip")

    **13.**

![alt_text](images/image15.png "image_tooltip")

    **14. - **


    **df -hT**

![alt_text](images/image16.png "image_tooltip")

    **15.**

![alt_text](images/image17.png "image_tooltip")

    **16.**

![alt_text](images/image18.png "image_tooltip")

    **17.**

![alt_text](images/image19.png "image_tooltip")

![alt_text](images/image20.png "image_tooltip")

    **	**


    **18.**

![alt_text](images/image21.png "image_tooltip")

    **19.**

![alt_text](images/image22.png "image_tooltip")

    **20.**

![alt_text](images/image23.png "image_tooltip")

![alt_text](images/image24.png "image_tooltip")


    **21. **

![alt_text](images/image25.png "image_tooltip")

    **22. **

![alt_text](images/image26.png "image_tooltip")

    **23. **


    **gedit /etc/fstab**

![alt_text](images/image27.png "image_tooltip")

![alt_text](images/image28.png "image_tooltip")

