> Iperf3 using interface: wlan0


##Server

>linaro@linaro-alip:~$ iperf3 -B wlan0 -s  

>Server listening on 5201  

>Accepted connection from xxx.xxx.xxx.xxx, port xxxxx  
>[   5] local xxx.xxx.xxx.xxx port 5201 connected to xxx.xxx.xxx.xxx port xxxxx  

| [  ID] | Interval | Transfer | Bandwidth |  
| ----- | -------- | --------:| ---------:|
| [ 5] | 0.00-1.00   sec | 4.56 MBytes | 38.3 Mbits/sec |
| [ 5] | 1.00-2.00   sec | 4.75 MBytes | 39.8 Mbits/sec |
| [ 5] | 2.00-3.00   sec | 4.78 MBytes | 40.1 Mbits/sec |
| [ 5] | 3.00-4.00   sec | 5.03 MBytes | 42.2 Mbits/sec |
| [ 5] | 4.00-5.00   sec | 5.08 MBytes | 42.6 Mbits/sec |
| [ 5] | 5.00-6.00   sec | 4.98 MBytes | 41.8 Mbits/sec |
| [ 5] | 6.00-7.00   sec | 5.07 MBytes | 42.5 Mbits/sec |
| [ 5] | 7.00-8.00   sec | 4.97 MBytes | 41.7 Mbits/sec |
| [ 5] | 8.00-9.00   sec | 5.02 MBytes | 42.1 Mbits/sec |
| [ 5] | 9.00-10.00  sec | 5.14 MBytes | 43.1 Mbits/sec |
| [ 5] | 10.00-10.04  sec |  249 KBytes | 46.5 Mbits/sec |
  

| [  ID] | Interval | Transfer | Bandwidth | / |
| ------ | -------- | --------:| ---------:| --- |
| [ 5] | 0.00-10.04  sec | 49.6 MBytes | 41.4 Mbits/sec | sender |
| [ 5] | 0.00-10.04  sec | 49.6 MBytes | 41.4 Mbits/sec | receiver |

>iperf3: interrupt - the server has terminated  


##Client

>linaro@linaro-alip:~$ iperf3 -B wlan0 -c xxx.xxx.xxx.xxx  

>Connecting to host xxx.xxx.xxx.xxx, port 5201  

>[   4] local xxx.xxx.xxx.xxx port xxxxx connected to xxx.xxx.xxx.xxx port 5201  

| [  ID] | Interval | Transfer | Bandwidth | Retr | Cwnd |
| ------ | -------- | --------:| ---------:|:----:| ---:|
| [ 4] | 0.00-1.00   sec |  246 KBytes | 2.02 Mbits/sec | 1 | 14.1 KBytes |
| [ 4] | 1.00-2.00   sec |  173 KBytes | 1.41 Mbits/sec | 0 | 14.1 KBytes |
| [ 4] | 2.00-3.00   sec |  206 KBytes | 1.69 Mbits/sec | 0 | 17.0 KBytes |
| [ 4] | 3.00-4.00   sec |  243 KBytes | 1.99 Mbits/sec | 0 | 19.8 KBytes |
| [ 4] | 4.00-5.00   sec |  194 KBytes | 1.59 Mbits/sec | 0 | 19.8 KBytes |
| [ 4] | 5.00-6.00   sec |  327 KBytes | 2.68 Mbits/sec | 0 | 22.6 KBytes |
| [ 4] | 6.00-7.00   sec |  250 KBytes | 2.05 Mbits/sec | 0 | 22.6 KBytes |
| [ 4] | 7.00-8.00   sec |  510 KBytes | 4.18 Mbits/sec | 0 | 28.3 KBytes |
| [ 4] | 8.00-9.00   sec |  557 KBytes | 4.56 Mbits/sec | 0 | 33.9 KBytes |
| [ 4] | 9.00-10.00  sec |  611 KBytes | 5.00 Mbits/sec | 0 | 36.8 KBytes |
  

| [  ID] | Interval | Transfer | Bandwidth | Retr | / |
| ------ | -------- | --------:| ---------:|:----:| --- |
| [ 4] | 0.00-10.00  sec | 3.24 MBytes | 2.72 Mbits/sec | 1 | sender
| [ 4] | 0.00-10.00  sec | 3.15 MBytes | 2.64 Mbits/sec | / | receiver

>iperf Done.  