<!-- Output copied to clipboard! -->

<!-- You have some errors, warnings, or alerts. If you are using reckless mode, turn it off to see inline alerts.
* ERRORs: 0
* WARNINGs: 0
* ALERTS: 15 -->

Lab 4

1 -   fdisk -l


![alt_text](images/image1.png "image_tooltip")


2 - 


![alt_text](images/image2.png "image_tooltip")


3 - 

To make sure that the changes applied we have to reboot or use command 

Partprobe

Sudo cat /proc/partitions


![alt_text](images/image3.png "image_tooltip")



![alt_text](images/image4.png "image_tooltip")


4 - mkfs .

Mkfs.ext2 /dev/sdc1


![alt_text](images/image5.png "image_tooltip")



![alt_text](images/image6.png "image_tooltip")


5 -  sudo mkdir /data

6 -  ntfslabel /dev/sdcl data


![alt_text](images/image7.png "image_tooltip")


7 - 

<span style="text-decoration:underline;">gedit /etc/fstab</span>

LABEL=data /data ext4 defaults 0 0

8 - => mount /dev/sdc1 /data/


![alt_text](images/image8.png "image_tooltip")


9 - 


![alt_text](images/image9.png "image_tooltip")


10 - 


![alt_text](images/image10.png "image_tooltip")


11 -


![alt_text](images/image11.png "image_tooltip")


12 -


![alt_text](images/image12.png "image_tooltip")


13 -


![alt_text](images/image13.png "image_tooltip")



![alt_text](images/image14.png "image_tooltip")



![alt_text](images/image15.png "image_tooltip")

