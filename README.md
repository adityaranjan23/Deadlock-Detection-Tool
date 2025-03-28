# Deadlock-Detection-Tool

## 📌 Overview

The **Automated Deadlock Detection Tool** is designed to monitor system processes and resources, detect potential deadlocks, and provide resolution options. It utilizes system calls, process monitoring, and graph-based cycle detection algorithms to analyze deadlock scenarios dynamically.

## 🚀 Features

- **Process & Resource Tracking:** Monitors system resources in real-time.
- **Graph-Based Deadlock Detection:** Uses cycle detection algorithms (DFS, Tarjan’s) for analysis.
- **Deadlock Resolution:** Suggests solutions like terminating processes or reallocating resources.
- **Automated Monitoring:** Runs periodically via cron jobs or system daemons.
- **Visualization & Logging:** Displays deadlock conditions and logs them for future reference.

## 🛠️ Technology Stack

### Programming Languages

- **Python** - For system monitoring and graph processing.
  

### Libraries and Tools
- **GitHub** - Version control and collaboration.
- **Linux /proc Filesystem** - For real-time process tracking.
- **Task Scheduler/Cron Jobs** - For automated execution.

## 📂 Project Structure

```
Deadlock-Detection-Tool/
│── src/                        # Source code
│   │── deadlock_detector.py    # Main Python script
│   │── utils/                   # Helper modules (if needed)
│── docs/                        # Documentation
│   │── project_report.md        # Detailed project report
│   │── flow_diagram.png         # High-level flow diagram
│── tests/                       # Test cases for the tool
│── logs/                        # Log files for deadlock incidents
│── README.md                    # Overview and instructions
│── requirements.txt              # Required dependencies
│── .gitignore                    # Ignore unnecessary files
│── LICENSE                       # Open-source license
```

## ⚙️ Installation

### Prerequisites

Ensure you have Python installed. Then, install the required dependencies:

```sh
pip install -r requirements.txt
```

### Running the Deadlock Detector

Run the script to start monitoring:

```sh
python src/deadlock_detector.py
```

### Example Output

```
🔍 Monitoring Processes for Deadlocks...
✅ No Deadlock Detected

🔍 Monitoring Processes for Deadlocks...
🔴 Deadlock Detected: [(1234, 'Memory_1024000'), ('Memory_1024000', 5678), (5678, 1234)]
🔴 Killing Process: 1234 to resolve deadlock
✅ Process 1234 Terminated Successfully
```

## 📌 Future Enhancements

- Implement GUI for better visualization.
- Support multi-resource allocation tracking.
- Use machine learning to predict deadlocks.

## 👨‍💻 Contributors

- Aditya Ranjan Behera
- Shorya Pratap Singh
- Rajat

