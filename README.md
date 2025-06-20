
# End-to-End-Medical-Chatbot-Generative-AI

## 🔧 How to Run?

### 🧪 Local Setup (Using Conda)

#### STEP 01 – Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

#### STEP 02 – Create and Activate Conda Environment

```bash
conda create -n medibot python=3.10 -y
conda activate medibot
```

#### STEP 03 – Install Python Dependencies

```bash
pip install -r requirements.txt
```

#### STEP 04 – Configure API Keys

Create a `.env` file in the root directory and add your Pinecone & OpenAI credentials:

```ini
PINECONE_API_KEY="xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
OPENAI_API_KEY="xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```

#### STEP 05 – Store Embeddings to Pinecone

```bash
python store_index.py
```

#### STEP 06 – Run the App

```bash
python app.py
```

Then open:

```bash
localhost:5000
```

---

## 🐳 Docker Setup (Recommended for Deployment)

### STEP 01 – Build the Docker Image

```bash
docker build -t medibot .
```

### STEP 02 – Run the Docker Container

```bash
docker run -d -p 5000:5000 --env-file .env medibot
```

* Make sure your `.env` file is in the same directory as the Dockerfile.

### STEP 03 – Access the Application

Visit:

```
http://localhost:5000
```

---

## 🛠 Tech Stack

* **Python**
* **LangChain**
* **Flask**
* **GPT (OpenAI)**
* **Pinecone**
* **Docker**

---

