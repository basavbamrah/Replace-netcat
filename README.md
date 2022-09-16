# Replace Netcat
<br>
Netcat is the utility knife of networking, it can be very useful for an attacker to find a way into network<br>
if we do not have netcat but have python installed on the server we can use this netcat replacement

## Example
> rp_netcat.py -t 192.168.1.108 -p 5555 -l -c # command shell<br>
>      rp_netcat.py -t 192.168.1.108 -p 5555 -l -u=mytext.txt # upload a file <br>
>       rp_netcat.py -t 192.168.1.108 -p 5555 -l -e=\"cat /etc/passwd\" # execute command  <br>
>        echo 'ABC' | ./rp_netcat.py -t 192.168.1.108 -p 135 # echo text to server port 135 <br>
>       rp_netcat.py -t 192.168.1.108 -p 555 # connect to server <br>


- Fire up two Terminals in first one create a listener using:
> python rp_netcat.py -t 127.0.0.1 -p 5555 -l -c
- On the sencond one type:
> python rp_netcat.py -t 127.0.0.1 -p 5555
