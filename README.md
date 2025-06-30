# cloud-monitoring-task2
Cloud Monitoring and Alerts using AWS CloudWatch.

# Internship Task-2: Cloud Monitoring and Alerts

## 🔍 Objective
Set up monitoring for a cloud-based application using **AWS CloudWatch** with configured alerts and a dashboard showcasing metrics.

---

## 🧰 Tools Used
- ✅ Amazon EC2 (as demo application)
- ✅ Amazon CloudWatch (monitoring and alerts)
- ✅ Amazon SNS (email notifications)
- ✅ AWS Console

---

## 🛠️ Steps Performed

### 1. Launched EC2 Instance
- Instance Name: `monitoring-demo`
- Type: `t2.micro` (Free Tier)
- Purpose: To act as a test application generating metrics like CPUUtilization.

### 2. Enabled CloudWatch Monitoring
- Default metrics (CPUUtilization, NetworkIn, etc.) enabled.
- Optional: CloudWatch Agent installed for advanced metrics.

### 3. Created CloudWatch Alarm
- Metric Monitored: **CPUUtilization**
- Threshold: Alert if CPU > 70% for 1 minute.
- Actions:
  - Created an **SNS Topic** named `cpu-alert-topic`.
  - Subscribed email address to receive alerts.
  - Received test email when threshold was crossed.

### 4. Built a CloudWatch Dashboard
- Dashboard Name: `EC2MonitoringDashboard`
- Widgets Added:
  - Line graph for CPUUtilization
  - NetworkIn & NetworkOut graphs
  - Alarm status widget

---

## ✅ Deliverables Summary

| Item                | Status |
|---------------------|--------|
| EC2 Instance Setup  | ✅     |
| CloudWatch Metrics  | ✅     |
| Alarm Setup         | ✅     |
| Dashboard Created   | ✅     |
| Email Alert Working | ✅     |

---

## 📌 Notes
I have to stop the EC2 instance to avoid Free Tier limits.

