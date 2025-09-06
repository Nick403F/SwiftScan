# SwiftScan v1

**SwiftScan** is Robust TCP Scanner with Banner Detection, Service Identification, Remote Logging, and Progress Tracking, it is also able to preform self destruct if specified.

---

##  Features

- Fast TCP port scanning with configurable port ranges
- Automatic service detection & banner grabbing
- Full HTTP/HTTPS header inspection for web services
- Local or remote logging of scan results
- Multi-threaded scanning for maximum speed
- Self-destruct/log-clean options for stealth
- Customizable service map (add new services easily)
- Real-time progress tracking

---

**Usage**

./swiftscan -t <target-ip> # basic scan

./swiftscan -t <target-ip> -a #scan every port

./swiftscan -t <target-ip> -p 1000:10000 -o scan_results.txt #scan ports from 1000 to 10000 and save results to file

./swiftscan -t <target-ip> -s target #sens scan results remotely to host 

./swiftscan --clean #self destructs #and clear its logs
Clone the repo:


**example output**

Port 8080 OPEN | Service: HTTP-Alt | Banner: N/A | HTTP Info:
HTTP/1.0 200 OK
Server: SimpleHTTP/0.6 Python/3.12.3
Date: Fri, 05 Sep 2025 22:37:13 GMT
Content-type: text/html; charset=utf-8
Content-Length: 351

---

##  Installation

```bash
git clone git@github.com:Nick403F/SwiftScan.git
cd SwiftScan
chmod +x swiftscan.sh



