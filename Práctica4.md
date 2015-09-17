# swap1415

# Práctica 4 : Comprobar el rendimiento de servidores web


![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P3/prueba_haproxy.png)


ab -n 1000 -c 10 192.168.56.10/script.php

Benchmarking 192.168.56.10 (be patient)
Completed 100 requests
Completed 200 requests
[...]
Finished 1000 requests


Server Software:        Apache/2.4.7
Server Hostname:        192.168.56.10
Server Port:            80

Document Path:          /script.php
Document Length:        18 bytes

Concurrency Level:      10
Time taken for tests:   2.551 seconds
Complete requests:      1000
Failed requests:        217
   (Connect: 0, Receive: 0, Length: 217, Exceptions: 0)
Total transferred:      204744 bytes
HTML transferred:       17744 bytes
Requests per second:    392.05 [#/sec] (mean)
Time per request:       25.507 [ms] (mean)
Time per request:       2.551 [ms] (mean, across all concurrent requests)
Transfer rate:          78.39 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    0   0.2      0       3
Processing:     3   25  15.0     19      81
Waiting:        3   23  13.7     18      81
Total:          3   25  15.0     20      83

Percentage of the requests served within a certain time (ms)
  50%     20
  66%     30
  75%     36
  80%     39
  90%     47
  95%     55
  98%     62
  99%     69
 100%     83 (longest request)
	 	