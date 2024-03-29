### Experiment Results: 



#### Methodology 

The Experiment conducted by measuring the request and access time for each of the instances for TEN times. Then the average is calculated. 

The result of the experiment is shown bellow in the chart. The blue bars are showing the average respond time for servers located in United States, "us-central-a" and orange bars shows the respond time for the servers located in South America "southamerica-a". The Experiment conducted using the Wi-Fi in University of Oklahoma, Norman, OK.

This Experiment conducted using the python script (https://github.com/agracy2246/RandomTiming) which is running in a Windows 10 Operating System. 

#### Observations

As Expected, there is a massive difference between the servers located in US and servers located in south America.  

![](/images/Chart.png)

The comparison between US servers shown in the chart bellow, with the fastest of VM java and slowest of App engine Java. 

![](images/Chart2.png)

And the results for South-America servers as follows: 

![](images/Chart3.png) 



#### Possible Errors

* This experiment used a python script running in a windows machine to conduct the experiment; therefore, the measured time may not be accurate reflection of the actual latency. Other processes running on the Operating System might caused extra latency measurements. 

* This experiment conducted using a Wi-Fi in a public network, in which might added extra latency.

* The servers that running VM and app-engines might not be in equal configuration in terms of dedicated hardware resources. 



### List of all Instances and numbers on the latest run

|       Region       |  Zone   |      Type      | Technology | Address                                            | Average Time In Microseconds |
| :----------------: | :-----: | :------------: | :--------: | :------------------------------------------------- | -------------------- |
|    us-central1     |    a    | Compute Engine |   Python   | http://34.66.236.240/                               | 61760.568   |
|      us-central1   |     a   | Compute Engine |    Java    | http://35.202.141.106/randNum/                      | 56172.03712 |
|      us-central1   | a       |   App Engine   |   Python   | http://pyrandomnumbergenerator.appspot.com/         | 59180.18818 |
|      us-central1   | a       |   App Engine   |    Java    | http://java-random-number-generator.appspot.com/demo| 66976.97639 |
| southamerica-east1 |    a    | Compute Engine |   python   | [http://34.95.171.137](http://34.95.171.137/)       | 291035.7237 |
| southamerica-east1 |    a    | Compute Engine |    Java    | http://34.95.224.56/randNum/                        | 298896.8611 |
| southamerica-east1 |    a    |   App Engine   |   Python   | https://timing-experiment-sa-zonea.appspot.com/     | 1203671.837 |
| southamerica-east1 |    a    |   App Engine   |    Java    | https://timing-experiment-sa-java.appspot.com/demo  | 502744.4363 |

### Experiments

The immediate output of the script for each run. 

The Order is as follows: 

1-US VM python

2-US VM Java

3-US App Engine python

4-US App Engine Java

5-SA VM python

6-SA VM Java

7-SA App Engine Python

8-SA App Engine Java 





Run 001:

```
it took 56819.68 microseconds to fetch from http://34.66.236.240/.
it took 50066.23 microseconds to fetch from http://35.202.141.106/randNum/.
it took 61851.74 microseconds to fetch from http://pyrandomnumbergenerator.appspot.com/.
it took 91921.57 microseconds to fetch from http://java-random-number-generator.appspot.com/demo.
it took 291191.82 microseconds to fetch from http://34.95.171.137.
it took 299172.40 microseconds to fetch from http://34.95.224.56/randNum/.
it took 1298527.72 microseconds to fetch from https://timing-experiment-sa-zonea.appspot.com/.
it took 245346.07 microseconds to fetch from https://timing-experiment-sa-java.appspot.com/demo
```

Run 002:

```
it took 55867.20 microseconds to fetch from http://34.66.236.240/.
it took 66793.44 microseconds to fetch from http://35.202.141.106/randNum/.
it took 53079.84 microseconds to fetch from http://pyrandomnumbergenerator.appspot.com/.
it took 54060.46 microseconds to fetch from http://java-random-number-generator.appspot.com/demo.
it took 289432.05 microseconds to fetch from http://34.95.171.137.
it took 294412.37 microseconds to fetch from http://34.95.224.56/randNum/.
it took 411900.28 microseconds to fetch from https://timing-experiment-sa-zonea.appspot.com/.
it took 1125961.07 microseconds to fetch from https://timing-experiment-sa-java.appspot.com/demo
```

Run 003:

```
it took 85772.75 microseconds to fetch from http://34.66.236.240/.
it took 50086.98 microseconds to fetch from http://35.202.141.106/randNum/.
it took 51834.11 microseconds to fetch from http://pyrandomnumbergenerator.appspot.com/.
it took 95743.66 microseconds to fetch from http://java-random-number-generator.appspot.com/demo.
it took 290225.03 microseconds to fetch from http://34.95.171.137.
it took 311167.00 microseconds to fetch from http://34.95.224.56/randNum/.
it took 1276551.01 microseconds to fetch from https://timing-experiment-sa-zonea.appspot.com/.
it took 1115952.97 microseconds to fetch from https://timing-experiment-sa-java.appspot.com/demo

```

Run 004:

```
it took 56848.29 microseconds to fetch from http://34.66.236.240/.
it took 50851.58 microseconds to fetch from http://35.202.141.106/randNum/.
it took 56070.57 microseconds to fetch from http://pyrandomnumbergenerator.appspot.com/.
it took 55049.66 microseconds to fetch from http://java-random-number-generator.appspot.com/demo.
it took 292229.89 microseconds to fetch from http://34.95.171.137.
it took 289200.07 microseconds to fetch from http://34.95.224.56/randNum/.
it took 1289553.40 microseconds to fetch from https://timing-experiment-sa-zonea.appspot.com/.
it took 228382.59 microseconds to fetch from https://timing-experiment-sa-java.appspot.com/demo
```

Run 005:

```
it took 58099.03 microseconds to fetch from http://34.66.236.240/.
it took 69889.55 microseconds to fetch from http://35.202.141.106/randNum/.
it took 75773.48 microseconds to fetch from http://pyrandomnumbergenerator.appspot.com/.
it took 66793.20 microseconds to fetch from http://java-random-number-generator.appspot.com/demo.
it took 290229.80 microseconds to fetch from http://34.95.171.137.
it took 295211.08 microseconds to fetch from http://34.95.224.56/randNum/.
it took 1286546.71 microseconds to fetch from https://timing-experiment-sa-zonea.appspot.com/.
it took 1089083.19 microseconds to fetch from https://timing-experiment-sa-java.appspot.com/demo
```

Run 006:

```
it took 56848.05 microseconds to fetch from http://34.66.236.240/.
it took 49614.67 microseconds to fetch from http://35.202.141.106/randNum/.
it took 59839.73 microseconds to fetch from http://pyrandomnumbergenerator.appspot.com/.
it took 66823.48 microseconds to fetch from http://java-random-number-generator.appspot.com/demo.
it took 291233.30 microseconds to fetch from http://34.95.171.137.
it took 291959.05 microseconds to fetch from http://34.95.224.56/randNum/.
it took 1291552.54 microseconds to fetch from https://timing-experiment-sa-zonea.appspot.com/.
it took 248348.00 microseconds to fetch from https://timing-experiment-sa-java.appspot.com/demo
```

Run 007:

```
it took 54865.12 microseconds to fetch from http://34.66.236.240/.
it took 49866.44 microseconds to fetch from http://35.202.141.106/randNum/.
it took 56849.00 microseconds to fetch from http://pyrandomnumbergenerator.appspot.com/.
it took 55896.04 microseconds to fetch from http://java-random-number-generator.appspot.com/demo.
it took 292196.99 microseconds to fetch from http://34.95.171.137.
it took 293220.28 microseconds to fetch from http://34.95.224.56/randNum/.
it took 1375329.73 microseconds to fetch from https://timing-experiment-sa-zonea.appspot.com/.
it took 253322.84 microseconds to fetch from https://timing-experiment-sa-java.appspot.com/demo
```

Run 008:

```
it took 56848.05 microseconds to fetch from http://34.66.236.240/.
it took 65822.60 microseconds to fetch from http://35.202.141.106/randNum/.
it took 51833.63 microseconds to fetch from http://pyrandomnumbergenerator.appspot.com/.
it took 58847.90 microseconds to fetch from http://java-random-number-generator.appspot.com/demo.
it took 293193.34 microseconds to fetch from http://34.95.171.137.
it took 291219.23 microseconds to fetch from http://34.95.224.56/randNum/.
it took 1258607.63 microseconds to fetch from https://timing-experiment-sa-zonea.appspot.com/.
it took 229384.66 microseconds to fetch from https://timing-experiment-sa-java.appspot.com/demo
```

Run 009:

```
it took 79785.11 microseconds to fetch from http://34.66.236.240/.
it took 59883.83 microseconds to fetch from http://35.202.141.106/randNum/.
it took 76796.77 microseconds to fetch from http://pyrandomnumbergenerator.appspot.com/.
it took 64814.57 microseconds to fetch from http://java-random-number-generator.appspot.com/demo.
it took 291197.30 microseconds to fetch from http://34.95.171.137.
it took 332180.74 microseconds to fetch from http://34.95.224.56/randNum/.
it took 1298490.05 microseconds to fetch from https://timing-experiment-sa-zonea.appspot.com/.
it took 270253.90 microseconds to fetch from https://timing-experiment-sa-java.appspot.com/demo
```

Run 10:

```
it took 55852.41 microseconds to fetch from http://34.66.236.240/.
it took 48845.05 microseconds to fetch from http://35.202.141.106/randNum/.
it took 47873.02 microseconds to fetch from http://pyrandomnumbergenerator.appspot.com/.
it took 59819.22 microseconds to fetch from http://java-random-number-generator.appspot.com/demo.
it took 289227.72 microseconds to fetch from http://34.95.171.137.
it took 291226.39 microseconds to fetch from http://34.95.224.56/randNum/.
it took 1249659.30 microseconds to fetch from https://timing-experiment-sa-zonea.appspot.com/.
it took 221409.08 microseconds to fetch from https://timing-experiment-sa-java.appspot.com/demo
```
