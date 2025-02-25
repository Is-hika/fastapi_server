**LET'S DIG IN !** 🚀🔥  

---

# ⚡ FastAPI Server with Docker & GitHub Actions 🐳  

![GitHub Workflow Status](https://github.com/Is-hika/fastapi_server/actions/workflows/main.yml/badge.svg)
![Docker](https://img.shields.io/badge/Docker-Supported-blue?style=for-the-badge&logo=docker)  
![FastAPI](https://img.shields.io/badge/FastAPI-UltraFast-green?style=for-the-badge&logo=fastapi)  
![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python)  

🚀 **A lightweight FastAPI server** with **Docker integration** and **automated deployment** using **GitHub Actions**.  

---

## 📂 Project Structure  

```bash
fastapi_server/
├── main.py              # FastAPI server
├── requirements.txt     # Python dependencies
├── Dockerfile           # Container configuration
├── .github/workflows/   # CI/CD configuration
└── README.md            # Project documentation
```

---

## 🛠️ Local Setup  

### ✅ Prerequisites  
- 🐍 **Python 3.8+**  
- 📦 **pip**  

### ⚙️ Installation  
1️⃣ Clone the repository:  
   ```bash
   git clone https://github.com/Is-hika/fastapi_server.git
   cd fastapi_server
   ```

2️⃣ Create a virtual environment:  
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use: venv\Scripts\activate
   ```

3️⃣ Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```

4️⃣ Run the application:  
   ```bash
   python main.py
   ```

5️⃣ Open your browser:  
   - 🌍 **API Base URL:** `http://localhost:8000`  
   - 📜 **Swagger UI:** [`http://localhost:8000/docs`](http://localhost:8000/docs)  

---

## 🐳 Docker Setup  

### 🔧 Build & Run Locally  
1️⃣ Build the Docker image:  
   ```bash
   docker build -t fastapi-server .
   ```

2️⃣ Run the container:  
   ```bash
   docker run -p 8000:8000 fastapi-server
   ```

3️⃣ Access the API at: [`http://localhost:8000`](http://localhost:8000)  

---

## 🚀 GitHub Actions CI/CD  

This project uses **GitHub Actions** to automate **Docker image builds** and **deployments** to **Docker Hub**.  

### 🔄 Workflow Steps  
✔️ Triggered on **every push**  
✔️ Sets up environment & dependencies  
✔️ Builds & pushes Docker image  
✔️ Deploys to **Docker Hub**  

### 🔐 Docker Hub Authentication  

1️⃣ **Generate a Docker Access Token**:  
   - Go to [Docker Hub](https://hub.docker.com/) → **Account Settings** → **Security** → **Access Tokens**  
   - Click **"New Access Token"**  
   - Copy the generated token  

2️⃣ **Add Token to GitHub Secrets**:  
   - Go to **GitHub → Repo → Settings → Secrets**  
   - Click **"New repository secret"**  
   - Name: `DOCKERTOKEN`  
   - Paste the **Docker Hub Token**  
   - Click **"Add secret"**  

---

## 📦 Docker Hub Image  

🛠️ **Pull the latest image** using:  
```bash
docker pull is-hika/fastapi-server:latest
```

---

## 🔥 API Endpoints  

| Method | Endpoint  | Description             |
|--------|----------|-------------------------|
| **GET**  | `/`        | Returns a welcome message |
| **GET**  | `/items`   | Returns a list of sample items |

---

## 💙 Contributing  

Contributions are welcome! Feel free to **fork** and submit a **pull request**. Let's build something great together! 🚀  

📩 **For queries or support:**  
📧 Email: ishika11082004@gmail.com  
🌐 [GitHub](https://github.com/Is-hika/fastapi_server)  

🔹 **Happy Coding!** 🎉🐍💡  