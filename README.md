## TODO

* create crontab script to run python on startup
* ansible
  * apt install rtl-sdr and python
  * copy python files
  * setup crontab
  * create user profile to contain and run python files




creating the kafka broker
https://www.digitalocean.com/community/tutorials/how-to-install-apache-kafka-on-ubuntu-20-04

install java

create a new user
sudo useradd kafka

download the latest binaries
https://downloads.apache.org/kafka/3.0.0/kafka_2.13-3.0.0.tgz

download and check the md5
https://downloads.apache.org/kafka/3.0.0/kafka_2.13-3.0.0.tgz.md5
md5sum kafka tgz === md5

make the kafka installation directory
mkdir -p /opt/kafka

give ownership to the kafka user
chown -r kafka /opt/kafka

extract the tgz into /opt/kafka
tar -xzf file.tgz

configure the KAFKA_HOME environment variable
(needs to go into kafka user shell config to persist after restart)

Create systemd services for zookeeper and kafka





## Getting Started

From the root directory, install all the role dependencies

```
ansible-galaxy install -r roles/requirements.yml
```

Run the playbook

```
ansible-playbook site.yml -kK
```
