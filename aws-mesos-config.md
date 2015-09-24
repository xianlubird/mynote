##AWS start mesos and marathon
1. start mesos master
```
bin/mesos-master.sh --ip=172.31.41.212 --work_dir=/home/ubuntu/tools/mesos-0.24.0/workdir
```

2. start mesos slave
```
bin/mesos-slave.sh --master=172.31.41.212:5050
```

3. start zookeeper
```
zkServer.sh start
```

4. start marathon
```
bin/start --master 172.31.41.212:5050 --zk zk://localhost:2181/marathon
```



