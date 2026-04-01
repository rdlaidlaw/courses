## grep
command: `grep 500 log.txt` <br>
output:<br>
```Bash
192.168.1.15 - - [01/Apr/2026:09:15:25] "GET /api/users" 500 312
192.168.1.15 - - [01/Apr/2026:09:17:00] "GET /api/users" 500 312
```

command: `grep 192.168.1.15 log.txt`<br>
output:
```Bash
192.168.1.15 - - [01/Apr/2026:09:15:25] "GET /api/users" 500 312
192.168.1.15 - - [01/Apr/2026:09:17:00] "GET /api/users" 500 312
```

## sed
command: `sed 's/192.168.1.15/192.168.1.15 (BANNED)/g' log.txt` - ban a user for getting a 500 error <br>
output:
```Bash
192.168.1.10 - - [01/Apr/2026:09:15:22] "GET /index.html" 200 1024
192.168.1.15 (BANNED) - - [01/Apr/2026:09:15:25] "GET /api/users" 500 312
10.0.0.5 - - [01/Apr/2026:09:15:30] "POST /login" 401 215
192.168.1.10 - - [01/Apr/2026:09:16:01] "GET /dashboard" 200 4096
10.0.0.5 - - [01/Apr/2026:09:16:05] "POST /login" 401 215
10.0.0.5 - - [01/Apr/2026:09:16:12] "POST /login" 200 512
192.168.1.15 (BANNED) - - [01/Apr/2026:09:17:00] "GET /api/users" 500 312
```

## awk
command: `` <br>
output:
```Bash

```