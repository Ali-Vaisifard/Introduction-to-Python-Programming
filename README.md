# Introduction-to-Python-Programming


## 🧑‍💻 Coding Environment Setup Guide 

This guide helps you set up a complete Python development environment including:

- Python
- Visual Studio Code
- Jupyter Notebook
- Docker

It is designed to work across different operating systems.

---

### 📦 1. Install Python

Download Python from the official website:

👉 https://www.python.org/downloads/

After installation, verify:

```bash
python --version
pip --version
```

---

### 💻 2. Install Visual Studio Code

Download VS Code:

👉 https://code.visualstudio.com/

After installation:

1. Open VS Code
2. Open Command Palette
3. Run:

```
Shell Command: Install 'code' command in PATH
```

---

### 🧩 3. Install VS Code Extensions

Install the following extensions:

- Python (Microsoft)
- Jupyter (Microsoft)
- Docker (Microsoft)

---

### 📁 4. Create Project

```bash
mkdir my_project
cd my_project
code .
```

---

### 🐍 5. Create Virtual Environment

```bash
python -m venv .venv
```

Activate it (command depends on your environment).

---

### 📦 6. Install Dependencies

```bash
python -m pip install --upgrade pip
pip install jupyterlab notebook ipykernel
```

---

### 📓 7. Setup Jupyter

Start Jupyter:

```bash
jupyter lab
```

Documentation:

👉 https://jupyter.org/install

---

### 🐳 8. Install Docker

Download Docker Desktop:

👉 https://www.docker.com/products/docker-desktop/

Verify:

```bash
docker --version
```

Test:

```bash
docker run hello-world
```

---

### 🧪 9. Basic Python Test

Create `main.py`:

```python
print("Environment ready!")
```

Run:

```bash
python main.py
```

---

### 📂 Project Structure

```
project/
├── src/
├── notebooks/
├── requirements.txt
├── Dockerfile
└── README.md
```

---

### 📦 10. Save Dependencies

```bash
pip freeze > requirements.txt
```

---

### 🐳 11. Example Dockerfile

```
FROM python:3.12-slim
WORKDIR /app
COPY . .
RUN pip install -r requirements.txt
CMD ["python", "main.py"]
```

---

### 🔄 Git Workflow

```bash
git init
git add .
git commit -m "Initial setup"
git push
```

Some othe commands to check out your git status: 

```bash
git status
git branch --show-current
git remote -v
git log --oneline -5
git push
```
Here is how to read the result:

 - git status should ideally say nothing to commit, working tree clean
 - git branch --show-current shows which branch you committed on
 - git remote -v shows which GitHub repository the Codespace is connected to
 - git log --oneline -5 shows whether your commit actually exists
 - git push sends the commit to GitHub if it has not been pushed yet

---

### ✅ You're Ready!

You now have:

- Python environment
- VS Code configured
- Jupyter working
- Docker ready

---

### 📬 Notes

- Always activate your virtual environment before working
- Use `requirements.txt` for reproducibility
- Keep your code organized

