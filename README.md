# 🪙 CoinDCX Trading Platform

A full-stack cryptocurrency trading dashboard built with React and Node.js using CoinDCX APIs. Place live market or limit orders using your CoinDCX credentials.

<br/>

## 📸 Preview

![UI Screenshot](./HomePage.png)

<br/>

## ⚙️ Tech Stack

- 🔥 React (Frontend)
- 🚀 Express.js (Backend)
- 🔐 CoinDCX API integration 
- 🗂️ Fullstack deployment-ready 

<br/>

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

<br/>

## 🚀 Features

- Live trade execution via CoinDCX
- Market / Limit orders
- Basic order form UI
- Server-side HMAC signing for secure requests
- Frontend served via backend for easy deployment

<br/>

## 🔐 Environment Variables

Create a .env file inside /backend:

```env
COINDCX_API_KEY=your_api_key
COINDCX_SECRET=your_api_secret
PORT=5000
```

👉 Note: You must complete KYC on CoinDCX to trade!

<br/>

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

<br/>



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

<br/>

## 📌 Notes

- This is a demo project. Use at your own risk.
- Trading APIs are real — keep your API key secure.
- No trading strategies are implemented.

<br/>

## 🤝 Contributing

Pull requests are welcome! For major changes, open an issue first to discuss what you'd like to change.

<br/>

## 📫 Contact

Made with 💙 by [Aditya Jatav](https://github.com/parth-jatav)
```

Let me know if you want me to tailor this for Vercel/Render deployment steps, or if you'd like a badge (e.g., build passing, license, etc.) added at the top!
