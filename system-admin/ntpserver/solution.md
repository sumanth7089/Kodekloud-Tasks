1 ssh into the server 

2 install ntp package

3 go to the ntp conf file vi /etc/ntp.conf and add the  server 3.europe.pool.ntp.org then save and exit (:wq)

4 check ntpstat

5 if it is not showing any result BTW it won't show any result it simpliy says Unable to talk to NTP daemon

6 then restart ntpd systemctl restart ntpd

7 then enable it systemctl enable ntpd

8 ntpstat

now it shows synchronised to NTP server (194.0.5.123) at stratum 3
   time correct to within 999 ms
   polling server every 64 s
 
