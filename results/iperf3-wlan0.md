> Iperf3 using interface: wlan0


##Server

>linaro@linaro-alip:~$ iperf3 -s  

>Server listening on 5201  

>Accepted connection from xxx.xxx.xxx.xxx, port xxxxx  
>[   5] local xxx.xxx.xxx.xxx port 5201 connected to xxx.xxx.xxx.xxx port xxxxx  

| [  ID] | Interval | Transfer | Bandwidth |  
| ----- | -------- | --------:| ---------:|
| [  5] |   0.00-1.00   sec |    163 KBytes |   1.33 Mbits/sec | 
| [  5] |   1.00-2.00   sec |   4.07 MBytes |   34.2 Mbits/sec | 
| [  5] |   2.00-3.00   sec |   3.97 MBytes |   33.3 Mbits/sec | 
| [  5] |   3.00-4.00   sec |   4.41 MBytes |   37.0 Mbits/sec | 
| [  5] |   4.00-5.00   sec |   4.53 MBytes |   38.0 Mbits/sec | 
| [  5] |   5.00-6.00   sec |   4.30 MBytes |   36.0 Mbits/sec | 
| [  5] |   6.00-7.00   sec |   4.37 MBytes |   36.6 Mbits/sec | 
| [  5] |   7.00-8.00   sec |   4.36 MBytes |   36.6 Mbits/sec | 
| [  5] |   8.00-9.00   sec |   4.42 MBytes |   37.1 Mbits/sec | 
| [  5] |   9.00-10.00  sec |   4.44 MBytes |   37.3 Mbits/sec | 
| [  5] |  10.00-10.05  sec |    226 KBytes |   34.0 Mbits/sec | 
  

| [  ID] | Interval | Transfer | Bandwidth | / |
| ------ | -------- | --------:| ---------:| --- |
| [  5] |   0.00-10.05  sec |   39.2 MBytes |   32.7 Mbits/sec | sender |
| [  5] |   0.00-10.05  sec |   39.2 MBytes |   32.7 Mbits/sec | receiver |

>iperf3: interrupt - the server has terminated  


##Client

>linaro@linaro-alip:~$ iperf3 -c xxx.xxx.xxx.xxx  

>Connecting to host xxx.xxx.xxx.xxx, port 5201  

>[   4] local xxx.xxx.xxx.xxx port xxxxx connected to xxx.xxx.xxx.xxx port 5201  

| [  ID] | Interval | Transfer | Bandwidth | Retr | Cwnd |
| ------ | -------- | --------:| ---------:|:----:| ---:|
| [  4] |   0.00-1.00   sec |   2.81 MBytes |   23.6 Mbits/sec |    16 | 73.5 KBytes | 
| [  4] |   1.00-2.00   sec |   3.77 MBytes |   31.6 Mbits/sec |     0 | 105 KBytes | 
| [  4] |   2.00-3.00   sec |   3.75 MBytes |   31.4 Mbits/sec |     0 | 127 KBytes | 
| [  4] |   3.00-4.00   sec |   3.81 MBytes |   32.0 Mbits/sec |     0 | 147 KBytes | 
| [  4] |   4.00-5.00   sec |   3.73 MBytes |   31.3 Mbits/sec |     0 | 165 KBytes | 
| [  4] |   5.00-6.00   sec |   3.59 MBytes |   30.1 Mbits/sec |     0 | 180 KBytes | 
| [  4] |   6.00-7.00   sec |   3.75 MBytes |   31.5 Mbits/sec |     0 | 195 KBytes | 
| [  4] |   7.00-8.00   sec |   3.62 MBytes |   30.4 Mbits/sec |     0 | 209 KBytes | 
| [  4] |   8.00-9.00   sec |   3.73 MBytes |   31.3 Mbits/sec |     0 | 209 KBytes | 
| [  4] |   9.00-10.00  sec |   3.64 MBytes |   30.5 Mbits/sec |     0 | 209 KBytes | 
  

| [  ID] | Interval | Transfer | Bandwidth | Retr | / |
| ------ | -------- | --------:| ---------:|:----:| --- |
| [  4] |   0.00-10.00  sec |   36.2 MBytes |   30.4 Mbits/sec | 16 | sender |
| [  4] |   0.00-10.00  sec |   36.1 MBytes |   30.3 Mbits/sec |  / | receiver |

>iperf Done.  