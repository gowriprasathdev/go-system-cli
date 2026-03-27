# 💻 System_CLI

A lightweight and efficient **System Resource Monitor** built with **Go (Golang)**. This CLI tool provides real-time information about your machine's CPU, Memory, and Disk utilization using a clean and intuitive interface.

## ✨ Features
*   **CPU Monitoring**: Quickly check current CPU usage percentage.
*   **Memory Insights**: get detailed information about RAM usage.
*   **Disk Status**: View disk space and usage statistics.
*   **Built for Speed**: Written in Go for minimal overhead and maximum performance.

## 🛠️ Technical Stack
*   **Language**: Go (Golang)
*   **CLI Framework**: [Cobra](https://github.com/spf13/cobra)
*   **System Metrics**: [gopsutil](https://github.com/shirou/gopsutil)

## 🚀 Installation & Usage

### 1. Prerequisites
*   Go 1.18 or higher installed.

### 2. Setup
Clone the repository and install dependencies:
```bash
git clone https://github.com/[your-username]/System_CLI.git
cd System_CLI
go mod tidy
```

### 3. Basic Commands
The tool uses the base command `system`. You can explore subcommands using:
```bash
go run main.go --help
```

#### Check CPU Usage:
```bash
go run main.go cpu
```

#### Check Memory Status:
```bash
go run main.go memory
```

#### Check Disk Space:
```bash
go run main.go disk
```

### 4. Global Installation (Optional)
To use the `system` command globally from any terminal, you can build the executable and move it to your system's `bin` directory:

```bash
# Build the binary
go build -o system

# Move to a directory in your PATH (e.g., /usr/local/bin or C:\bin)
# On Linux/macOS:
mv system /usr/local/bin/

# On Windows:
# Move 'system.exe' to a folder included in your System PATH
```

Now you can simply run:
```bash
system cpu
```

## 📂 Project Structure
*   `main.go`: Entry point for the application.
*   `cmd/`: Contains the command logic for `cpu`, `memory`, and `disk`.
*   `go.mod`: Project dependencies.

---
*Built with ❤️ using Go.*
