- Check for multiple NICs on compromised system, look for other networks to pivot to
- ipconfig, ifconfig, netstat -r, ip route etc
  ### SSH local port forwarding
  ![image](https://github.com/nationalcptc-teamtools/Coastline-College/assets/85032657/caddd47b-800d-4b8b-8a87-11344eabcd05)

  - use SSH to forward port on remote host to local port
    ```
    ssh -L <local port>:localhost:<remote port> <username>@<ip>
     ```
  - to check if forwarding is being done
    ```
    netstat -antp | grep <local port>
     ```
    ```
    nmap -v -p <local port> localhost
    ```
### SSH tunneling over SOCKS proxy
  #### proxychains
  ![image](https://github.com/nationalcptc-teamtools/Coastline-College/assets/85032657/952c6e3e-2842-440f-848c-b9c1c03e5756)

  - Use SSH dynamic port forwarding
  ```
    ssh -D 9050 <username>@<ip>
   ```
```
  /etc/proxychains.conf
```
