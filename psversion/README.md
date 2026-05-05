# AKS Monitoring & Observability - Hands-on Lab (PowerShell Version)

This folder contains the **PowerShell-friendly** version of the AKS Monitoring & Observability labs. All bash commands have been converted to PowerShell syntax.

## 📚 Chapters

| # | Chapter | Link |
|---|---------|------|
| 0 | Setup and Prerequisites | [README](./chapter-0-setup/README.md) |
| 1 | Azure Monitor + Container Insights | [README](./chapter-1-azure-monitor/README.md) |
| 2 | Azure Managed Prometheus + Grafana | [README](./chapter-2-prometheus-grafana/README.md) |
| 3 | PromQL Basics + Alerting | [README](./chapter-3-promql-alerting/README.md) |
| 4 | Metrics Collection & Visualization | [README](./chapter-4-metrics-comparison/README.md) |
| 5 | Cost Optimization for Metrics Ingestion | [README](./chapter-5-cost-optimization/README.md) |

## 🔧 Requirements

- **PowerShell 7+** (Windows PowerShell or PowerShell Core)
- **Azure CLI** (`az`)
- **kubectl**
- **Helm** (v3.x)

## 🚀 Getting Started

Start with **[Chapter 0: Setup and Prerequisites](./chapter-0-setup/README.md)** and complete each chapter in sequence.

## 📝 Key Differences from Bash Version

| Bash | PowerShell |
|------|-----------|
| `export VAR="value"` | `$VAR = "value"` |
| `source ./file.sh` | `. ./file.ps1` |
| `\` line continuation | `` ` `` backtick continuation |
| `sleep 30` | `Start-Sleep -Seconds 30` |
| `echo "text"` | `Write-Host "text"` |
| `cmd \| grep pattern` | `cmd \| Select-String pattern` |
| `$(command)` subshell | `$(command)` or `$var = command` |
| Heredoc `<<EOF` | Here-string `@" ... "@` |

> **Note**: `kubectl` and `az` CLI commands work identically in both shells. PromQL and KQL queries are unchanged — they are query languages, not shell syntax.
