## ffuf
- use cookies
```bash
ffuf -b "NAME1=VALUE1; NAME2=VALUE2" -w wordlist.txt -u https://host.name/FUZZ
```