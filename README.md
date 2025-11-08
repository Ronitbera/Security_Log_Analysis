# 🧩 Security Log Analysis – Cybersecurity Mini Project

## 📖 Overview
This project analyzes simulated server log data using Python to detect suspicious login activities, such as brute-force attempts and unusual access patterns. It demonstrates the application of data analytics for cybersecurity monitoring — aligning with cyber risk detection and incident response processes.

## 🧠 Objective
To identify and visualize abnormal login patterns from system logs using Python, Pandas, and Matplotlib.

## ⚙️ Tools & Libraries
- Python
- Pandas
- Matplotlib
- Datetime

## 📁 Dataset
The dataset (`server_logs.csv`) contains simulated login records:
| timestamp | username | ip_address | status |
|------------|-----------|------------|---------|
| 2025-11-08 09:01:22 | admin | 192.168.0.5 | Failed |
| 2025-11-08 09:02:03 | admin | 192.168.0.5 | Failed |
| 2025-11-08 09:02:42 | admin | 192.168.0.5 | Success |

## 💻 Steps Performed
1. Loaded and cleaned server log data using Pandas.  
2. Detected brute-force attacks based on repeated failed logins.  
3. Identified unusual login times (midnight to 5 AM).  
4. Visualized top IPs with failed login attempts.

## 📊 Visualization Example
```python
failed_logins['ip_address'].value_counts().head(10).plot(kind='bar')
