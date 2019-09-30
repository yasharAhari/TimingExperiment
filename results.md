### Experiment Results: 



### List of all Instances and numbers on the latest run

|       Region       |  Zone   |      Type      | Technology | Address                                            | Time In Microseconds |
| :----------------: | :-----: | :------------: | :--------: | :------------------------------------------------- | -------------------- |
|    us-central1     |    a    | Compute Engine |   Python   | http://34.66.236.240/                              | missing              |
|      us-central1   |     a   | Compute Engine |    Java    | http://35.202.141.106/randNum/                     | missing              |
|      us-central1   | a |   App Engine   |   Python   | http://pyrandomnumbergenerator.appspot.com/              | missing              |
|      us-central1       | a |   App Engine   |    Java    | http://java-random-number-generator.appspot.com/demo                                            | missing              |
| southamerica-east1 |    a    | Compute Engine |   python   | [http://34.95.171.137](http://34.95.171.137/)      | 366023.06            |
| southamerica-east1 |    a    | Compute Engine |    Java    | http://34.95.224.56/randNum/  | missing              |
| southamerica-east1 |    a    |   App Engine   |   Python   | https://timing-experiment-sa-zonea.appspot.com/    | 1214754.10           |
| southamerica-east1 |    a    |   App Engine   |    Java    | https://timing-experiment-sa-java.appspot.com/demo | 593413.35            |



#### Before Changing zones: 

WOW, SUCH EMPTY 

#### After Changing Zones

Run 001:

```
it took 366023.06 microseconds to fetch from http://34.95.171.137/.
it took 593413.35 microseconds to fetch from https://timing-experiment-sa-java.appspot.com/demo.
it took 1214754.10 microseconds to fetch from https://timing-experiment-sa-zonea.appspot.com/.
```

|       Region       | Zone |    App\|VM     | Technology | Time in microseconds |
| :----------------: | :--: | :------------: | :--------: | -------------------- |
| southamerica-east1 |  a   | Compute Engine |   Python   | 366023.06            |
| southamerica-east1 |  a   |   App Engine   |    Java    | 593413.35            |
| southamerica-east1 |  a   |   App Engine   |   Python   | 1214754.10           |
| southamerica-east1 |  a   | Compute Engine |    Java    | missing!             |

