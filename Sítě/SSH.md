# Cisco SSH

```
nable

conf t

hostname R2

enable secret cisco

line console 0

password cisco

login

exit

ip domain-name ssps.cz

cryp k g r

1024

username maty secret maty

line vty 0 15

transport input ssh

login local

exit

exit

copy run start
```
