# flink-on-hdfs
- Setup and a WordCount application on a distributed Apache Flink installation using Apache Hadoop (HDFS).
## Requirements
- Google Cloud Account
- Google Cloud SDK set up
- first, setup 3 GCP nodes using the SDK. We used Ubuntu 18.04 as OS on e2-standard-4 machines (4 vCPUs, 16 GB Mem). Smaller ones might work, but can face ressource problems with heavier tasks. The nodes have to be in the same subnetwork.
- configure ssh access to the VMs from local host and between the VMs. This task is described in previous assignments and skipped here
- install `wget`, `java8` and `pdsh`
## Usage
- This is how to deploy the application
### Deployment
- run `./cluster.sh`. This will start the Hadoop cluster and Apache Flink on the GCP VMs.

