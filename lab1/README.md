<!-- Output copied to clipboard! -->

<!-- You have some errors, warnings, or alerts. If you are using reckless mode, turn it off to see inline alerts.
* ERRORs: 0
* WARNINGs: 0
* ALERTS: 20 -->

**Lab 1**

**1 - systemctl status**


![alt_text](images/image1.png "image_tooltip")


**2- **

**= > <code>systemctl set-default graphical.target</code></strong>

** **


![alt_text](images/image2.png "image_tooltip")


**3 - 4**

**Echo “Test” | mail -s “Test” root**

**Su -s root**


![alt_text](images/image3.png "image_tooltip")


**5 - **


![alt_text](images/image4.png "image_tooltip")
** \
**

**6 - 7**


![alt_text](images/image5.png "image_tooltip")


**8 - 9**


![alt_text](images/image6.png "image_tooltip")


**13 -**

**lp -d tty12 /etc/hosts**

**lpstat tty12**
![alt_text](images/image7.png "image_tooltip")


**14 -**

**cupsdisable tty12**


![alt_text](images/image8.png "image_tooltip")


**15 -**

** lp -d tty12 /etc/hosts**

**Sudo lp -d tty12 /etc/xinetd.conf**


![alt_text](images/image9.png "image_tooltip")


**16 -**

**lpq -a**

**lpq -P tty12**


![alt_text](images/image10.png "image_tooltip")



![alt_text](images/image11.png "image_tooltip")


**17 -**

**cancel tty12-2**

**cupsenable tty12**


![alt_text](images/image12.png "image_tooltip")



![alt_text](images/image13.png "image_tooltip")


**18 -**

**cupsreject tty12**


![alt_text](images/image14.png "image_tooltip")


**19 -**

**lp -d tty12 /etc/hosts**

**lp: Destination "tty12" is not accepting jobs.**


![alt_text](images/image15.png "image_tooltip")


**20 -**

**lpadmin -x tty12**

**// caneneled **


![alt_text](images/image16.png "image_tooltip")


**21 - **

**crontab -e **

***/10 8-17 08 12 4**


![alt_text](images/image17.png "image_tooltip")


**22 - **


![alt_text](images/image18.png "image_tooltip")


**23 - **


![alt_text](images/image19.png "image_tooltip")


**24 - **


![alt_text](images/image20.png "image_tooltip")

