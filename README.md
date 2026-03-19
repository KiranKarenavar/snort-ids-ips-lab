# 🛡️ Snort IDS/IPS Lab

## 📌 Overview

This project demonstrates the implementation of **Snort** as an Intrusion Detection System (IDS) and provides an overview of its capability to function as an Intrusion Prevention System (IPS).

Snort is an open-source network security tool used to monitor, detect, and prevent malicious activities in network traffic.

---

## 🎯 Objectives

* To understand the working of Snort
* To configure Snort as an IDS
* To analyze network traffic and detect threats
* To study Snort’s IPS capabilities (inline mode)

---

## 🧰 Tools & Technologies Used

* Snort
* Linux (Ubuntu/Kali)
* Command Line Interface (CLI)
* Network Interface (eth0)

---

## 🔍 Snort as IDS (Intrusion Detection System)

Snort was configured in IDS mode to:

* Monitor network traffic
* Detect suspicious/malicious packets
* Generate alerts and logs

### ▶️ Sample Command

```
snort -A console -q -c /etc/snort/snort.conf -i eth0
```

### 📊 Features

* Real-time traffic analysis
* Packet logging
* Rule-based detection

---

## 🛡️ Snort as IPS (Intrusion Prevention System)

Snort can also function as an IPS when configured in **inline mode**.

### ⚙️ Key Points:

* Works inline with network traffic
* Can block/drop malicious packets
* Uses DAQ (Data Acquisition Library)

### ▶️ Example Command (Inline Mode)

```
snort -Q --daq afpacket -c /etc/snort/snort.conf -i eth0
```

> ⚠️ Note: IPS mode was studied conceptually and not fully implemented in this project.

---

## 📸 Screenshots

Screenshots of alerts and configurations are included in the `screenshots/` folder.

---

## 📂 Lab Structure

```
snort-ids-project/
│── report/
│── screenshots/
│── README.md
```

---

## ⚖️ IDS vs IPS

| Feature    | IDS     | IPS    |
| ---------- | ------- | ------ |
| Detection  | ✅       | ✅      |
| Prevention | ❌       | ✅      |
| Deployment | Passive | Inline |

---

## 🚀 Conclusion

Snort is a powerful tool for network security. In this project, it was successfully implemented as an IDS to detect network threats. Additionally, its IPS capability was explored, showing that Snort can also prevent attacks when configured in inline mode.

---

## 👤 Author

* Kiran Karenavar

---
