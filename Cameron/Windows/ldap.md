# check for anonymous bind
## nmap 
```bash
nmap --script=ldap-search.nse -p 389 192.168.220.102
```
## ldapsearch
### enumerate the base of objects
#### works for basic auth (non GSSAPI, kerberos) and ldap...change things up like port and ldaps:// for ldaps
```bash
ldapsearch -H ldap://192.168.220.102 -x -b '' "(objectClass=*)"
```
### then drill down to specific containers like...
```
ldapsearch -H ldap://192.168.220.102 -x -b "CN=Users,DC=cptc,DC=localnet"
ldapsearch -H ldap://192.168.220.102 -x -b "OU=IT Tier 1,DC=cptc,DC=localnet" "(objectClass=user)" sAMAccountName
```


