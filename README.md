# 💰 Xpensify

A modern, AI-powered personal finance management platform built with Next.js 15 and React 19. Track your expenses, manage budgets, and gain insights into your financial habits with intelligent automation.

## ✨ Features

- **🔐 Secure Authentication** - Powered by Clerk for seamless sign-in/sign-up
- **💳 Account Management** - Create and manage multiple financial accounts
- **📊 Transaction Tracking** - Add, categorize, and monitor your transactions
- **📈 Budget Management** - Set budgets and track your spending progress
- **🤖 AI-Powered Receipt Scanner** - Extract transaction data from receipts using Google Gemini AI
- **📧 Email Notifications** - Automated email alerts and reports via Resend
- **🛡️ Security & Rate Limiting** - Protected by Arcjet security features
- **📱 Responsive Design** - Beautiful UI with Tailwind CSS and Radix UI components
- **🌙 Dark/Light Mode** - Theme switching with next-themes
- **📊 Data Visualization** - Interactive charts and graphs with Recharts

## 🚀 Tech Stack

### Frontend
- **Next.js 15** - React framework with App Router
- **React 19** - Latest React with concurrent features
- **Tailwind CSS** - Utility-first CSS framework
- **Radix UI** - Accessible component primitives
- **Framer Motion** - Smooth animations and transitions
- **Lucide React** - Beautiful icon library

### Backend & Database
- **Prisma** - Type-safe database ORM
- **PostgreSQL** - Robust relational database (Supabase)
- **Inngest** - Background job processing

### Authentication & Security
- **Clerk** - Complete authentication solution
- **Arcjet** - Security and rate limiting
- **Zod** - Runtime type validation

### AI & External Services
- **Google Gemini AI** - Receipt scanning and data extraction
- **Resend** - Transactional email service

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Anurag1023/Xpensify.git
   cd Xpensify
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env` file in the root directory:
   ```env
   DATABASE_URL="your_database_url"
   DIRECT_URL="your_direct_database_url"

   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY="your_clerk_publishable_key"
   CLERK_SECRET_KEY="your_clerk_secret_key"
   NEXT_PUBLIC_CLERK_SIGN_IN_URL="/sign-in"
   NEXT_PUBLIC_CLERK_SIGN_UP_URL="/sign-up"
   NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL="/onboarding"
   NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL="/onboarding"

   GEMINI_API_KEY="your_gemini_api_key"
   RESEND_API_KEY="your_resend_api_key"
   ARCJET_KEY="your_arcjet_key"
   ```

4. **Set up the database**
   ```bash
   npx prisma generate
   npx prisma db push
   ```

5. **Run the development server**
   ```bash
   npm run dev
   ```

   Open [http://localhost:3000](http://localhost:3000) to view the application.

## 📁 Project Structure

```
├── app/                    # Next.js App Router
│   ├── (auth)/            # Authentication routes
│   ├── (main)/            # Main application routes
│   ├── api/               # API routes
│   └── lib/               # App-specific utilities
├── components/            # Reusable UI components
│   └── ui/               # Base UI components
├── lib/                  # Shared utilities and configurations
├── prisma/               # Database schema and migrations
├── actions/              # Server actions
├── hooks/                # Custom React hooks
├── data/                 # Static data and configurations
└── emails/               # Email templates
```

## 🎯 Key Features Explained

### Account Management
- Create multiple accounts (checking, savings, credit cards)
- View account balances and transaction history
- Interactive charts showing spending patterns

### Transaction Tracking
- Manual transaction entry with categorization
- AI-powered receipt scanning for automatic data extraction
- Search and filter transactions
- Export transaction data

### Budget Management
- Set monthly budgets by category
- Track spending progress with visual indicators
- Receive notifications when approaching budget limits

### Security Features
- Rate limiting to prevent abuse
- Secure authentication with Clerk
- Data validation with Zod schemas
- HTTPS enforcement and security headers

## 🚀 Deployment

### Vercel (Recommended)
1. Push your code to GitHub
2. Connect your repository to Vercel
3. Add environment variables in Vercel dashboard
4. Deploy!

### Manual Deployment
```bash
npm run build
npm start
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Scripts

- `npm run dev` - Start development server with Turbopack
- `npm run build` - Build for production
- `npm start` - Start production server
- `npm run lint` - Run ESLint
- `npm run email` - Start email development server

## 🔧 Environment Setup

### Required Services
1. **Supabase** - PostgreSQL database hosting
2. **Clerk** - Authentication service
3. **Google AI Studio** - Gemini API access
4. **Resend** - Email service
5. **Arcjet** - Security and rate limiting

## 📊 Database Schema

The application uses Prisma with PostgreSQL, supporting:
- User accounts and profiles
- Financial accounts (checking, savings, etc.)
- Transactions with categories
- Budget tracking
- Email notifications

## 🎨 UI Components

Built with:
- **Radix UI** - Accessible primitives
- **Tailwind CSS** - Styling
- **Class Variance Authority** - Component variants
- **Lucide React** - Icons
- **Recharts** - Data visualization

## 📱 Responsive Design

Fully responsive design that works seamlessly across:
- Desktop browsers
- Tablets
- Mobile devices

## 🐛 Known Issues

- Email development requires additional setup
- Some features may require specific API quotas

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- [Next.js](https://nextjs.org/) - The React framework
- [Clerk](https://clerk.com/) - Authentication made easy
- [Prisma](https://www.prisma.io/) - Database toolkit
- [Tailwind CSS](https://tailwindcss.com/) - CSS framework
- [Radix UI](https://www.radix-ui.com/) - UI primitives

---

Made with ❤️ by [shivansh746](https://github.com/shivansh746)
