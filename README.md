# Azure Self-Healing Infra AI Agent

An end-to-end AI-powered **Azure Infrastructure Self-Healing platform** that:
- Monitors Azure VMs and resources
- Uses an AI Agent (Azure OpenAI) to **diagnose issues**
- Suggests and optionally **executes self-healing actions**
- Provides a **web dashboard** for visibility and manual control

---

## 🚀 Features

- Azure VM health monitoring (CPU, heartbeat, connectivity)
- AI-powered incident diagnosis using Azure OpenAI
- Self-healing actions (e.g., NSG fixes, VM restart)
- Incident history stored in Azure Storage
- React + TypeScript dashboard for visualization
- REST API built with FastAPI
- Deployed to Azure App Service + Azure Static Web Apps
- Secure integration via Managed Identity & Key Vault

---

## 🧱 Architecture

- **Frontend**: React + TypeScript (Vite) hosted on Azure Static Web Apps  
- **Backend**: FastAPI (Python) on Azure App Service  
- **AI**: Azure OpenAI (gpt-4o) with tool/function calling  
- **Monitoring**: Azure Monitor + Log Analytics  
- **Storage**: Azure Storage (Table/Blob) for incidents  
- **Security**: Managed Identity + Azure Key Vault  
- **Notifications**: Microsoft Teams via Incoming Webhook (optional)


---

## 📂 Project Structure

```text

backend/   # FastAPI app
frontend/  # React + TS app
infra/     # Bicep templates & pipelines
docs/      # Architecture, API spec, workflows
