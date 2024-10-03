# 🛠️ **CI/CD Automation with Jenkins and Selenium** 🛠️

This project is a **Java-based tool** for CI/CD, utilizing **Jenkins** as a standalone automation server. The architecture follows a **Master-Slave** model, with developers continuously integrating their work via **GitHub**, and automated tests and deployments are handled using **Selenium**.

---

## **🌍 Architecture Overview**

1. **Developers** push code changes to the **GitHub Repository** 🗃️.
2. **Jenkins** (Automation Tool) 🖥️ polls the repository for updates and triggers the build process.
3. **Selenium** 🧪 executes automated tests.
4. Successfully built and tested applications are **Deployed** 🚀 to the appropriate environment.

---

## **🔄 Jenkins Master-Slave Setup**

- **Master Node** handles scheduling and distribution of jobs.
- **Slave Nodes** (Windows, Mac, Linux) handle build and execution tasks.

The architecture ensures that the heavy lifting of the build is distributed across multiple platforms for efficient execution.

---

## **📋 Jenkins CI Process**

1. Developers commit code to the **GitHub Repo**.
2. **Jenkins Server** polls for changes and triggers automated builds.
3. **Selenium** is used for end-to-end testing.
4. Deployment occurs after a successful build and test cycle.

---

## **🔧 Virtual Environment Setup**

To run tests and automate the environment, follow the steps below to set up a Python virtual environment.

### **1. Create Virtual Environment**

```bash
python -m venv .venv
```

### **2. Activate Environment (Windows)**

```bash
Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
.\.venv\Scripts\Activate.ps1
```

### **3. Install Dependencies**

```bash
pip install -r requirements.txt
```

docker run -p 8080:8080 -p 5000:5000 -v jenkins_home:home/Anas/jenkins_home --name -d jenkins/jenkins:lts
