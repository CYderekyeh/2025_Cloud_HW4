# 2025cloud App

This is a demo Node.js application for TSMC container deployment assignment.

## 🐳 How to Build Docker Image

```bash
docker build -t derekyeh901018/2025cloud:ver1 .
```
## 🐳 How to Run Docker Image

```bash
docker run derekyeh901018/2025cloud:ver1
```

---

## 📦 自動化產生 Container Image 的流程說明

本專案使用 GitHub Actions 自動化產生容器映像檔 (Docker Image)，流程如下：

```mermaid
graph TD
  A[推送程式碼至 main 分支] --> B[GitHub Actions 自動觸發]
  B --> C[執行 docker build 建立 Image]
  C --> D[將 Image 推送至 Docker Hub 2025cloud Repo]
