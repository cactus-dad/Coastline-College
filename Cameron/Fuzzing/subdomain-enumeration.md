## ffuf
```bash
ffuf -H "Host: FUZZ.domain.name" -w /path/to/wordlist/ -u www.url.com -fs <content lengths to filter out>
```