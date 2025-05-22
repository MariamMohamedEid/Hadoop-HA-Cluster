# Hadoop-HA-Cluster
# Hadoop High Availability (HA) Cluster with Docker

This project sets up a High Availability Hadoop cluster using Docker and ZooKeeper. It features:
- 3 NameNodes (for HA using ZooKeeper & JournalNodes)
- 3 ResourceManagers (for YARN HA)
- Multiple DataNodes and NodeManagers
- Fully Dockerized infrastructure for reproducibility and ease of deployment

## 🔧 Components

- **HDFS**: Configured with HA using three NameNodes.
- **YARN**: Configured with ResourceManager HA.
- **ZooKeeper**: Ensures leader election and failover.
- **Docker + Docker Compose**: Container orchestration.

---

## 🗂 Directory Structure

![image](https://github.com/user-attachments/assets/fc42dc5f-0e3d-42bd-8e14-52341a794d36)


---

## 🧱 Cluster Architecture

### Master Nodes
Each master node runs:
- NameNode or Standby NameNode
- ResourceManager (HA)
- ZooKeeper
- JournalNode

### Worker Nodes
Each worker runs:
- DataNode
- NodeManager

