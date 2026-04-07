# 📘 Math Discord Bot (AI-Powered)

An AI-powered Discord bot designed to solve mathematical problems for students, especially **A/L Combined Maths** level.

Supports:

* Step-by-step solutions
* Fast answers
* Image-based math questions (via AI vision)

---

## 🚀 Features

* 🧠 AI-based math solving (Hugging Face + OpenRouter)
* 📊 Step-by-step explanations
* ⚡ Fast answer mode
* 🖼️ Image-to-text (OCR for math questions)
* 🔄 Automatic fallback if one model fails
* 🧹 Clean formatted output (no messy LaTeX)

---

## 🛠️ Tech Stack

* Node.js
* Discord.js
* Hugging Face Inference API
* OpenRouter (fallback for better models)
* Axios

---

## 📦 Installation

### 1. Clone the repo

```bash
git clone https://github.com/your-username/math-discord-bot.git
cd math-discord-bot
```

### 2. Install dependencies

```bash
npm install
```

### 3. Setup environment variables

Create a `.env` file:

```env
HF_TOKEN=your_huggingface_token
HF_MATH_MODEL=Qwen/Qwen2.5-7B-Instruct
HF_OCR_MODEL=Salesforce/blip2-opt-2.7b

OPENROUTER_API_KEY=your_openrouter_key
```

---

## ▶️ Running the Bot

```bash
node index.js
```

---

## 💬 Commands

### Solve with steps

```bash
!hfmath solve <question>
```

### Step-by-step explanation

```bash
!hfmath steps <question>
```

### Fast answer only

```bash
!hfmath fast <question>
```

### With image

Upload an image with the command:

```bash
!hfmath solve
```

---

## 🧪 Example

**Input:**

```
!hfmath solve integrate ln(x)/(x^2+1) from 0 to infinity
```

**Output:**

```
Problem:
Evaluate ∫ from 0 to ∞ of ln(x)/(x² + 1) dx

Steps:
Using substitution x = 1/t, the integral becomes the negative of itself.

So:
I = -I
2I = 0
I = 0

Final Answer: 0
```

---

## ⚙️ Configuration

You can change models in `.env`:

* `HF_MATH_MODEL` → main text model
* `HF_OCR_MODEL` → image processing model

---

## ⚠️ Limitations

* Free-tier models may give inconsistent answers
* Complex integrals may require fallback models
* OCR may fail on unclear images

---

## 🔥 Future Improvements

* ✅ Answer verification system
* ✅ Multiple model comparison
* ✅ Web dashboard for usage tracking
* ✅ Premium faster model support

---

## 🤝 Contributing

Pull requests are welcome. For major changes, open an issue first.

---

## 📄 License

MIT License

---

## 💡 Author

Built by a student, for students — focused on making math easier with AI.
