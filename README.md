

# 🧠 Welth – AI-Powered Finance Platform

![Welth Banner](public/banner.jpeg)

**Welth** is a modern, AI-powered personal finance management platform built with **Next.js 14**, offering real-time transaction tracking, intelligent budgeting, and actionable financial insights.

---

## 🌟 Features

### 💳 Account Management

* Create and manage multiple account types (Savings, Current, etc.)
* Real-time balance tracking
* Detailed analytics and trends per account

### 💰 Transaction Management

* Record and categorize income/expenses
* Support for recurring transactions (Daily/Weekly/Monthly/Yearly)
* Upload and scan receipts with AI-powered data extraction
* Advanced filtering and search for transaction history

### 📊 Budget Management

* Set monthly budgets with category-based allocations
* Interactive visualizations for budget progress
* Real-time budget alerts and spend tracking

### 📈 Financial Analytics

* Insightful visual reports with Recharts
* Monthly/yearly expense breakdowns
* Track income vs. expense trends

### 🤖 AI-Powered Intelligence

* Smart insights powered by **Gemini AI**
* Auto-categorize transactions
* Personalized financial recommendations
* OCR-based receipt extraction

### 📧 Automated Notifications

* Monthly summary emails
* Budget threshold alerts
* Transaction reminders
* Account activity notifications

### 🔒 Security and Compliance

* Secure auth with **Clerk**
* API rate limiting via **ArcJet**
* Environment variable protection
* Connection pooling and production-level DB optimization

---

## 🚀 Tech Stack

| Layer        | Tech Used                                 |
| ------------ | ----------------------------------------- |
| **Frontend** | Next.js 14, React, Tailwind CSS, Radix UI |
| **Backend**  | Next.js API Routes, Prisma ORM            |
| **Database** | PostgreSQL (Supabase)                     |
| **Auth**     | Clerk                                     |
| **AI/ML**    | Google Gemini API                         |
| **Email**    | Resend                                    |
| **Security** | ArcJet                                    |
| **Charts**   | Recharts                                  |
| **Forms**    | React Hook Form, Zod                      |

---

## 📦 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/sukanta-chowdhury/Welth.git
cd Welth
```

### 2. Install dependencies

```bash
npm install
```

### 3. Set up environment variables

Create a `.env` file in the root directory:

```env
# Supabase DB
DATABASE_URL="your_database_url"
DIRECT_URL="your_direct_url"

# Clerk Auth
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

# AI Services
GEMINI_API_KEY=your_gemini_api_key

# Email (Resend)
RESEND_API_KEY=your_resend_api_key

# Security
ARCJET_KEY=your_arcjet_key
```

### 4. Initialize the database

```bash
npx prisma generate
npx prisma db push
```

### 5. Start development server

```bash
npm run dev
```

Visit: [http://localhost:3000](http://localhost:3000)

---

## 🛠 Development Commands

| Command         | Description                 |
| --------------- | --------------------------- |
| `npm run dev`   | Start development server    |
| `npm run build` | Build the production app    |
| `npm run start` | Start the production server |
| `npm run lint`  | Run ESLint checks           |
| `npm run email` | Preview emails with Resend  |

---

## 📡 API Documentation

### 🔐 Auth

* `GET /api/auth/*` – Clerk auth endpoints
* `POST /api/inngest/*` – Background job triggers

### 🔄 Transactions

* `POST /api/transactions` – Create a transaction
* `GET /api/transactions` – Fetch transactions
* `PUT /api/transactions/:id` – Update a transaction
* `DELETE /api/transactions/:id` – Delete a transaction

### 🏦 Accounts

* `POST /api/accounts` – Create a new account
* `GET /api/accounts` – List all accounts
* `PUT /api/accounts/:id` – Edit an account
* `DELETE /api/accounts/:id` – Remove an account

### 📅 Budgets

* `POST /api/budgets` – Create/Update budgets
* `GET /api/budgets` – Get budget data

---

## 🤝 Contributing

1. Fork the repo
2. Create a feature branch: `git checkout -b feature/myFeature`
3. Commit your changes: `git commit -m 'Add myFeature'`
4. Push to GitHub: `git push origin feature/myFeature`
5. Create a Pull Request

---

## 📄 License

Licensed under the [MIT License](LICENSE)

---

## 👥 Authors & Collaborators

| Name                  | GitHub                                                     |
| --------------------- | ---------------------------------------------------------- |
| **Sukanta Chowdhury** | [@sukanta-chowdhury](https://github.com/sukanta-chowdhury) |
| **SK Mirajul Islam**  | [@skmirajulislam](https://github.com/skmirajulislam)       |

---

## 🙏 Acknowledgements

* [Next.js](https://nextjs.org/)
* [Clerk](https://clerk.dev/)
* [Supabase](https://supabase.com/)
* [Google Gemini AI](https://ai.google.dev/gemini)
* [Resend](https://resend.com/)
* All OSS contributors & maintainers

---

## 📞 Support

For queries, reach us at **[support@welth.com](mailto:skmirajulislaqm181@gmail.com)** or join our **Slack workspace**.
