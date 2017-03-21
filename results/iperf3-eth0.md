> Iperf3 using interface: eth0


##Server

>linaro@linaro-alip:~$ iperf3 -s  

>Server listening on 5201  

>Accepted connection from xxx.xxx.xxx.xxx, port xxxxx  
>[   5] local xxx.xxx.xxx.xxx port 5201 connected to xxx.xxx.xxx.xxx port xxxxx  

| [  ID] | Interval | Transfer | Bandwidth |  
| ----- | -------- | --------:| ---------:|
| [   5] | 0.00-1.00   sec | 106 MBytes |    889 Mbits/sec
| [   5] | 1.00-2.00   sec | 111 MBytes |    933 Mbits/sec
| [   5] | 2.00-3.00   sec | 112 MBytes |    942 Mbits/sec
| [   5] | 3.00-4.00   sec | 112 MBytes |    942 Mbits/sec
| [   5] | 4.00-5.00   sec | 112 MBytes |    942 Mbits/sec
| [   5] | 5.00-6.00   sec | 112 MBytes |    942 Mbits/sec
| [   5] | 6.00-7.00   sec | 112 MBytes |    942 Mbits/sec
| [   5] | 7.00-8.00   sec | 112 MBytes |    941 Mbits/sec
| [   5] | 8.00-9.00   sec | 111 MBytes |    933 Mbits/sec
| [   5] | 9.00-10.00  sec | 112 MBytes |    942 Mbits/sec 
| [   5] | 10.00-10.00  sec | 235 KBytes | 907 Mbits/sec
  

| [  ID] | Interval | Transfer | Bandwidth | / |
| ------ | -------- | --------:| ---------:| --- |
| [   5] | 0.00-10.00  sec | 1.09 GBytes | 935 Mbits/sec | sender |
| [   5] | 0.00-10.00  sec | 1.09 GBytes | 935 Mbits/sec | receiver |

>iperf3: interrupt - the server has terminated  


##Client

>linaro@linaro-alip:~$ iperf3 -c xxx.xxx.xxx.xxx  

>Connecting to host xxx.xxx.xxx.xxx, port 5201  

>[   4] local xxx.xxx.xxx.xxx port xxxxx connected to xxx.xxx.xxx.xxx port 5201  

| [  ID] | Interval | Transfer | Bandwidth | Retr | Cwnd |
| ------ | -------- | --------:| ---------:|:----:| ---:|
| [   4] | 0.00-1.00   sec | 98.1 MBytes |    823 Mbits/sec |   0 | 221 KBytes  
| [   4] | 1.00-2.00   sec |  104 MBytes |    869 Mbits/sec |   0 | 221 KBytes  
| [   4] | 2.00-3.00   sec |  107 MBytes |    894 Mbits/sec |   0 | 221 KBytes  
| [   4] | 3.00-4.00   sec |  108 MBytes |    903 Mbits/sec |   0 | 221 KBytes  
| [   4] | 4.00-5.00   sec |  109 MBytes |    915 Mbits/sec |   0 | 221 KBytes  
| [   4] | 5.00-6.00   sec |  104 MBytes |    873 Mbits/sec |   0 | 221 KBytes  
| [   4] | 6.00-7.00   sec |  107 MBytes |    895 Mbits/sec |   0 | 221 KBytes  
| [   4] | 7.00-8.00   sec |  106 MBytes |    886 Mbits/sec |   0 | 221 KBytes  
| [   4] | 8.00-9.00   sec |  105 MBytes |    879 Mbits/sec |   0 | 221 KBytes  
| [   4] | 9.00-10.00  sec |  105 MBytes |    878 Mbits/sec |   0 | 221 KBytes  
  

| [  ID] | Interval | Transfer | Bandwidth | Retr | / |
| ------ | -------- | --------:| ---------:|:----:| --- |
| [   4] | 0.00-10.00  sec | 1.03 GBytes | 882 Mbits/sec | 0 | sender |
| [   4] | 0.00-10.00  sec | 1.03 GBytes | 881 Mbits/sec | / | receiver |

>iperf Done.  