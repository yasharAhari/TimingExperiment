## Timing Experiment 

### How to move a VM to other region and zones in Google Could 

For this operation, you need to have an already existing google cloud VM. You can create a new one using the instruction [here](https://github.com/ZachArani/RandomNumberGCP).

#### Snapshot

To start, we create a snapshot of the existing VM, for this,

* Login to your google cloud console,  

* Click the Menu button (Three line) and select the ```Compute Engine```

* On the left menu select ```Snapshots```

  ![Select Snapshots](.\images\GoToSnapShots.png)

* Now Press ```Create Snapshot``` on to menu bar

  ![Select Create Snapshot](images\SelectCreate.png)

* Enter the desired configuration and select your existing VM to create snapshot of that VM.

  ![Enter Configuration](images\DoSettings.png)  

* After Configuring, press create and wait until the snapshot created.

#### Create a new VM by that Snapshot

* On the snapshot page, select the snapshot we just created

  ![select snapshot](images\SelectTheSnapShot.png)

* And now press ``` Create Instance ``` on top menu

  ![Select Create Instance ](images\SelectCreate.png)

* And now insert the desired configuration for new instance. 

  * Word of advice: Make sure the new instance is same or at least has higher machine configuration as the snapshot instance 

     ![Configure](F:\projects\softwereEngin\exp\TimingExperiment\images\SettingTheVM.png)

* Here, you can select the new Region and Zone as marked above.

* After configuring, select ```create```.  

  Congratulations! Now you have a new instance with other VM's snapshot. It means all your installations, configuration and files will be in new instance too.
