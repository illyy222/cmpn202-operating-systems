Week 6 – Performance Evaluation and Analysis

CMPN202 Operating Systems Coursework
Ilhan Mohamed – A00023555

📌 Overview

Week 6 focused on evaluating the performance of the Ubuntu Server under different workloads and analysing how the operating system behaves when system resources are stressed. The aim was to measure CPU usage, observe system behaviour under load, and identify potential bottlenecks. All performance testing was carried out on the Ubuntu Server via SSH, with monitoring performed in parallel to reflect real-world system administration practices.

Baseline Performance Testing

Before applying any workload, a baseline measurement was taken to understand how the system behaves under normal conditions. The top command was used to observe CPU usage, memory usage, and running processes while the system was idle.

This baseline provided a reference point for comparing performance once stress testing was applied.

Evidence:
Baseline monitoring screenshots are available in the week6-images folder.

CPU Load Testing

To simulate a CPU-intensive workload, the stress tool was used to generate sustained CPU load on the Ubuntu Server. This allowed observation of how the operating system schedules processes and manages CPU resources under pressure.

While the stress test was running in one terminal session, a second terminal session was opened to monitor real-time system performance using top. This showed a clear increase in CPU utilisation and confirmed that the stress processes were actively consuming CPU resources.

Evidence:
Screenshots showing CPU stress execution and real-time monitoring output are available in the week6-images folder.

Performance Monitoring and Observation

During the load test, system responsiveness and process behaviour were monitored closely. The operating system successfully handled the increased workload without crashing or becoming unresponsive. CPU usage increased significantly during the stress test and returned to normal once the test was stopped, demonstrating effective process scheduling and resource management by the OS.

Multiple screenshots were captured to document:

Baseline system state

Active CPU stress testing

Real-time monitoring output

Evidence:
All monitoring and stress test screenshots are stored in the week6-images folder.

Issues Encountered and Troubleshooting

One challenge encountered during this week was managing multiple terminal sessions simultaneously while ensuring the correct commands were being monitored at the right time. Initially, there was confusion about whether monitoring should be done from Linux Mint or Ubuntu. This was resolved by understanding that performance monitoring must occur directly on the Ubuntu Server while the workload is running.

Additionally, managing terminal windows and capturing clear screenshots required careful coordination to ensure outputs were visible and readable.

Analysis and Findings

The results showed that the Ubuntu Server handled CPU-intensive workloads effectively. CPU utilisation increased as expected during stress testing, while system stability was maintained throughout. Once the workload ended, the system returned to baseline performance levels, indicating efficient resource management and scheduling by the operating system.

This testing demonstrated how operating systems prioritise processes and manage system resources dynamically under load.

Reflection

Week 6 improved my understanding of how operating systems behave under performance stress and how to measure this using command-line tools. Running stress tests alongside real-time monitoring helped me clearly see the relationship between workload and system resource usage. Troubleshooting session management and monitoring timing also strengthened my confidence in performing performance analysis tasks that reflect real-world system administration scenarios.
