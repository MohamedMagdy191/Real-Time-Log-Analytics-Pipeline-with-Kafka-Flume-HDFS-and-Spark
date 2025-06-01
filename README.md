# ⚙️ Real-Time Log Analytics Pipeline with Kafka, Flume, HDFS, and Spark

This project implements a **real-time log processing pipeline** using:

- **Apache Kafka** for high-throughput log ingestion  
- **Apache Flume** for log data collection and movement  
- **Hadoop (HDFS)** for distributed data storage  
- **Apache Spark** for real-time and batch data processing  

---

## 📌 Objective

To build a **scalable and efficient pipeline** that collects, transports, stores, and analyzes logs in real-time, enabling **advanced monitoring** and **insight into system/application behavior**.

---

## 🧱 Components Overview

- **Kafka**  
  Acts as the **message broker** to handle streaming log data.

- **Flume**  
  Collects logs from source systems and **pushes them into Kafka or HDFS**.

- **HDFS**  
  Stores log data in a **fault-tolerant, distributed** environment.

- **Spark**  
  Processes stored logs for **analytics**, **pattern detection**, or **alerting**.

---

## 💡 Use Cases

- Monitoring server or application logs  
- Detecting anomalies or errors in real-time  
- Generating analytics dashboards or reports  

---

## 📂 Repository Contents

| File | Description |
|------|-------------|
| `GenLogs.py` | Python script to generate sample log data |
| `Kafka-to-hdfs.conf` | Flume configuration for sending Kafka data to HDFS |
| `file-to-kafka.conf` | Flume configuration for sending log files to Kafka |
| `Sparkaf.py` | Spark application to process log data from HDFS |
| `Commands.docx` | Setup and usage command reference |
| `Workflow.md` | Detailed description of the pipeline workflow |
| `Readme.md` | This file |

---

## 🚀 Getting Started

To run the pipeline:

1. Start Kafka and Zookeeper
2. Start Flume agents with the provided config files
3. Run `GenLogs.py` to generate log data
4. Use Spark (`Sparkaf.py`) to process logs from HDFS

> Refer to `Commands.docx` and `Workflow.md` for setup and execution details.

---

## 🛠️ Requirements

- Apache Kafka  
- Apache Flume  
- Hadoop (HDFS)  
- Apache Spark  
- Python 3.x  

---
