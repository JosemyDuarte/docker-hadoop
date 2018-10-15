# **hadoop**
___

### Description

This image runs the [*Cloudera CDH Hadoop*](https://www.cloudera.com/products/open-source/apache-hadoop/key-cdh-components.html) in a **pseudo-distributed** mode on a Centos 7 Linux distribution.

The *latest* tag of this image is build with the latest available release of CDH on Centos 7.

You can pull it with:

    docker pull josemyd/hadoop

Run with Docker Compose:

    docker-compose up

Once started you'll be able to read the list of all the Hadoop Web GUIs urls:

| **Hadoop Web UIs**        |**URL**                            |
|:--------------------------|:----------------------------------|
| *Hadoop Name Node*        | http://localhost:50070            |
| *Hadoop Data Node*        | http://localhost:50075            |
| *YARN Node Manager*       | http://localhost:8042             |
| *YARN Resource Manager*   | http://localhost:8088             |
| *YARN Timeline History*   | http://localhost:8188             |
| *MapReduce Job History*   | http://localhost:19888/jobhistory |

While the Hadoop Docker container is running, you can always get the urls' list with the script:

    print-urls.sh

included in the GitHub source repository.

### Copyright

This image is based on the work of [Parrot Stream](https://github.com/parrot-stream/docker-hadoop/)