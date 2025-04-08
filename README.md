# 🧠 Phidata Agent Playground

This project demonstrates how to build interactive AI agents using [Phidata](https://phidata.app/) with FastAPI and local session storage. It includes two example agents: a **Web Agent** (for online search) and a **Finance Agent** (for stock and company info).

---

## 🚀 Features

- 🌍 **Web Agent**: Uses DuckDuckGo to answer questions with sources.
- 📈 **Finance Agent**: Uses Yahoo Finance to display stock prices, company news, and recommendations in table format.
- 🧩 Local session storage using SQLite
- ⚡ Beautiful UI with `Agent Playground` powered by FastAPI

---

## 📦 Requirements

- Python 3.10+
- [Phidata CLI](https://docs.phidata.app/)
- [FastAPI](https://fastapi.tiangolo.com/)
- [SQLite3](https://sqlite.org/)

---

## 🧪 Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/arpitpatelsitapur/Agents-using-PhiData.git
cd Agents-using-PhiData
```

### 2. Create Virtual Environment (Recommended)

Avoid version conflicts with other AI libraries like LangChain or LlamaIndex:

```bash
python -m venv phi-env
source phi-env/bin/activate  # On Mac/Linux
# For Windows:
# phi-env\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -U pip
pip install phidata
pip install "fastapi[all]" sqlalchemy
```

### 4. Authenticate with Phidata

```bash
phi auth
```

A browser window will open for you to log in via phidata.app.

### 5. Run the Playground

```bash
python playground.py
```

Then open the browser at:
http://localhost:7777 and select localhost:7777 from the dropdown.

---

## 🧩 File Structure

```
playground.py    # Main app entry point
agents.db        # SQLite database to store agent conversations
```

---

## 🛠 Troubleshooting

- **Pydantic version issues**? Ensure you're using pydantic>=2.7,<3 for compatibility with Phidata.
- Use a **clean virtual environment** to avoid dependency conflicts with other libraries.

---

## 🧠 Bonus Tip

If you're mixing a lot of AI libraries (LangChain, LlamaIndex, Phidata, etc.), consider using a clean virtual environment for Phidata:

```bash
python -m venv phi-env
source phi-env/bin/activate  # On Mac/Linux
# For Windows:
# phi-env\Scripts\activate
pip install -U pip
pip install phidata
pip install "fastapi[all]" sqlalchemy
```

---

## 📄 License

MIT License © 2025 Arpit Patel

---

## 🙌 Credits

Thanks to the Phidata team for this awesome framework!
