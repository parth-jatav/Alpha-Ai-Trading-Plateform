


# 🪙 CoinDCX Trading Platform

A full-stack cryptocurrency trading dashboard built with React and Node.js using CoinDCX APIs. Place live market or limit orders using your CoinDCX credentials.

## 📸 Preview

![UI Screenshot](./HomePage.png)

---

## ⚙️ Tech Stack

- 🔥 React + Vite (Frontend)
- 🚀 Express.js (Backend)
- 🔐 CoinDCX API integration (HMAC SHA256 signed requests)
- 🗂️ Fullstack deployment-ready (Render / Railway / Fly.io)

---

## 📁 Project Structure

```
project-root/
│
├── frontend/         # React frontend
│   ├── src/
│   └── build/        # React build output (served by Express)
│
├── backend/          # Express backend
│   ├── server.js     # API routes and static file server
│   ├── public/       # Optional static files (favicon, images)
│   └── .env          # CoinDCX secrets (not committed)
│
└── README.md
```

---

## 🚀 Features

- Live trade execution via CoinDCX
- Market / Limit orders
- Basic order form UI
- Server-side HMAC signing for secure requests
- Frontend served via backend for easy deployment

---

## 🔐 Environment Variables

Create a .env file inside /backend:

```env
COINDCX_API_KEY=your_api_key
COINDCX_SECRET=your_api_secret
PORT=5000
```

👉 Note: You must complete KYC on CoinDCX to trade!

---

## 🛠️ Getting Started Locally

### 1. Clone Repo

```bash
git clone https://github.com/your-username/coindcx-trade-app.git
cd coindcx-trade-app
```

### 2. Install & Build Frontend

```bash
cd frontend
npm install
npm run build
```

### 3. Setup & Run Backend

```bash
cd ../backend
npm install
node server.js
```

Visit ➡️ http://localhost:5000

---

## 📦 Deployment Options

✅ Option A: Fullstack on Render

- Build React inside /frontend
- Backend serves /frontend/build
- One-click deploy from GitHub

✅ Option B: Split Frontend (Vercel) + Backend (Render)

- Deploy frontend with Vercel (link /frontend folder)
- Deploy backend to Render separately
- Connect via API URL in React

Want a full deployment guide? → Ask in the issues tab or contribute one!

---

## 📄 API

Backend endpoint for placing trades:

| Method | Endpoint       | Description            |
|--------|----------------|------------------------|
| POST   | /place-order   | Place a new trade      |

Payload example:

```json
{
  "market": "BTCINR",
  "side": "buy",
  "order_type": "market",
  "quantity": 0.01
}
```

---

## 📌 Notes

- This is a demo project. Use at your own risk.
- Trading APIs are real — keep your API key secure.
- No trading strategies are implemented.

---

## 🤝 Contributing

Pull requests are welcome! For major changes, open an issue first to discuss what you'd like to change.

---

## 📜 License

MIT License

---

## 📫 Contact

Made with 💙 by [Your Name](https://github.com/your-username)
```

Let me know if you want me to tailor this for Vercel/Render deployment steps, or if you'd like a badge (e.g., build passing, license, etc.) added at the top!
