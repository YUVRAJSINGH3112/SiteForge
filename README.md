# 🚀 SiteForge

**SiteForge** is an AI-powered website builder built with the **MERN Stack** that allows users to generate and build modern websites using natural language.

Instead of starting from scratch, users can describe what they want to build, and SiteForge uses AI to help generate the website structure and content.

---

## ✨ Features

* 🤖 AI-powered website generation
* 💬 Generate websites using natural language prompts
* ⚡ Modern and responsive UI
* 🔐 User authentication with JWT
* 🗄️ MongoDB database
* 🌐 MERN Stack architecture
* 🔑 Secure environment-based configuration
* 🧠 OpenRouter API integration
* 📱 Responsive website generation
* 🛠️ Separate client and server architecture

---

## 🏗️ Tech Stack

### Frontend

* React.js
* Vite
* JavaScript
* CSS / Tailwind CSS

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT Authentication

### AI

* OpenRouter API
* Configurable OpenRouter AI Model

---

## 📁 Project Structure

```text
SiteForge/
│
├── client/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── .env
│
├── server/
│   ├── src/
│   ├── package.json
│   └── .env
│
└── README.md
```

---

# ⚙️ Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/YUVRAJSINGH3112/SiteForge.git
```

Navigate into the project:

```bash
cd SiteForge
```

---

## 2. Install Dependencies

### Backend

```bash
cd server
npm install
```

### Frontend

Open another terminal:

```bash
cd client
npm install
```

---

# 🔐 Environment Variables

SiteForge requires environment variables for both the **server** and **client**.

## Backend `.env`

Create a `.env` file inside the `server` folder:

```env
JWT_SECRET=your_jwt_secret

ORIGINS=http://localhost:5173

MONGODB_URI=your_mongodb_connection_string

OPENROUTER_API_KEY=your_openrouter_api_key

OPENROUTER_MODEL=your_openrouter_model
```

### Backend Environment Variables

| Variable             | Description                            |
| -------------------- | -------------------------------------- |
| `JWT_SECRET`         | Secret key used for JWT authentication |
| `ORIGINS`            | Frontend URL allowed by the backend    |
| `MONGODB_URI`        | MongoDB database connection string     |
| `OPENROUTER_API_KEY` | API key for OpenRouter                 |
| `OPENROUTER_MODEL`   | AI model used through OpenRouter       |

---

## Frontend `.env`

Create a `.env` file inside the `client` folder:

```env
VITE_API_URL=http://localhost:5000
```

> Change the URL according to your backend deployment.

---

# ▶️ Running the Project

SiteForge has two separate applications:

* `client` → Frontend
* `server` → Backend

You need to run both.

## Start Backend

From the project root:

```bash
cd server
npm install
npm run dev
```

The backend will start on the configured server port.

---

## Start Frontend

Open a **new terminal**:

```bash
cd client
npm install
npm run dev
```

Vite will provide a local URL, usually:

```text
http://localhost:5173
```

Open the URL in your browser to use SiteForge.

---

# 🔄 Development Workflow

Run both applications simultaneously:

### Terminal 1 — Server

```bash
cd server
npm run dev
```

### Terminal 2 — Client

```bash
cd client
npm run dev
```

---

# 🔒 Security

Never commit your `.env` files or expose API keys publicly.

Make sure your `.gitignore` contains:

```gitignore
node_modules/
.env
.env.local
dist/
```

Especially keep your:

* MongoDB credentials
* JWT secret
* OpenRouter API key

private.

---

# 🤖 AI Architecture

SiteForge uses **OpenRouter** to communicate with AI models.

The AI model can be configured through:

```env
OPENROUTER_MODEL=your_openrouter_model
```

This allows the AI model to be changed without modifying the application code.

---

# 🚧 Project Status

**Active Development**

SiteForge is currently under development and new AI-powered website generation capabilities are being added.

---

# 👨‍💻 Author

**Yuvraj Singh**

GitHub: [YUVRAJSINGH3112](https://github.com/YUVRAJSINGH3112)

---

## ⭐ Support

If you find SiteForge interesting, consider giving the repository a ⭐ on GitHub.
