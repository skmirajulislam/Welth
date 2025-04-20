# Welth - AI-Powered Finance Platform

![Welth Banner](public/banner.jpeg)

Welth is a modern, AI-powered finance management platform built with Next.js 14, featuring real-time transaction tracking, budget management, and intelligent financial insights.

## 🌟 Features

### 💳 Account Management
- Create and manage multiple financial accounts
- Track account balances in real-time
- View detailed account statistics and trends
- Support for different account types (Current, Savings)

### 💰 Transaction Management
- Record income and expenses with detailed categorization
- Recurring transaction support (Daily, Weekly, Monthly, Yearly)
- Receipt scanning and automatic data extraction
- Transaction history with advanced filtering and search
- Real-time balance updates

### 📊 Budget Management
- Set and track monthly budgets
- Visual progress tracking with interactive charts
- Automated budget alerts and notifications
- Category-wise budget allocation

### 📈 Financial Analytics
- Interactive charts and visualizations
- Expense categorization and analysis
- Income vs. Expense tracking
- Monthly and yearly financial reports

### 🤖 AI-Powered Features
- Smart financial insights using Google's Gemini AI
- Automated receipt data extraction
- Personalized financial recommendations
- Intelligent categorization of transactions

### 📧 Automated Notifications
- Monthly financial report emails
- Budget threshold alerts
- Recurring transaction reminders
- Account activity notifications

### 🔒 Security Features
- Secure authentication with Clerk
- Rate limiting with ArcJet
- Database connection pooling
- Environment variable protection

## 🚀 Tech Stack

- **Frontend**: Next.js 14, React, TailwindCSS
- **Backend**: Next.js API Routes, Prisma
- **Database**: PostgreSQL (via Supabase)
- **Authentication**: Clerk
- **Email**: Resend
- **AI/ML**: Google Gemini AI
- **Security**: ArcJet
- **Styling**: Tailwind CSS, Radix UI
- **Charts**: Recharts
- **Forms**: React Hook Form, Zod

## 📦 Installation

1. Clone the repository:
\`\`\`bash
git clone https://github.com/sukanta-chowdhury/Welth.git
cd Welth
\`\`\`

2. Install dependencies:
\`\`\`bash
npm install
\`\`\`

3. Set up environment variables:
Create a \`.env\` file in the root directory with the following variables:
\`\`\`env
# Database URLs (Supabase)
DATABASE_URL="your_database_url"
DIRECT_URL="your_direct_url"

# Clerk Authentication
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

# AI Services
GEMINI_API_KEY=your_gemini_api_key

# Email Service
RESEND_API_KEY=your_resend_api_key

# Security
ARCJET_KEY=your_arcjet_key
\`\`\`

4. Run database migrations:
\`\`\`bash
npx prisma generate
npx prisma db push
\`\`\`

5. Start the development server:
\`\`\`bash
npm run dev
\`\`\`

The application will be available at `http://localhost:3000`

## 🛠️ Development Commands

- `npm run dev` - Start development server
- `npm run build` - Build production version
- `npm run start` - Start production server
- `npm run lint` - Run ESLint
- `npm run email` - Start email preview server

## 📝 API Documentation

### Authentication Endpoints
- `/api/auth/*` - Clerk authentication endpoints
- `/api/inngest/*` - Background job processing

### Transaction Endpoints
- POST `/api/transactions` - Create new transaction
- GET `/api/transactions` - List transactions
- PUT `/api/transactions/:id` - Update transaction
- DELETE `/api/transactions/:id` - Delete transaction

### Account Endpoints
- POST `/api/accounts` - Create new account
- GET `/api/accounts` - List accounts
- PUT `/api/accounts/:id` - Update account
- DELETE `/api/accounts/:id` - Delete account

### Budget Endpoints
- POST `/api/budgets` - Create/update budget
- GET `/api/budgets` - Get budget information

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/AmazingFeature`
3. Commit your changes: `git commit -m 'Add some AmazingFeature'`
4. Push to the branch: `git push origin feature/AmazingFeature`
5. Open a pull request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- Sukanta Chowdhury - [GitHub Profile](https://github.com/sukanta-chowdhury)

## 🙏 Acknowledgments

- Next.js team for the amazing framework
- Clerk for authentication
- Supabase for database hosting
- Google for Gemini AI
- All other open-source contributors

## 📞 Support

For support, email support@welth.com or join our Slack channel.
