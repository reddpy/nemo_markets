# Nemo Markets IP CRM

> An AI-powered CRM for intellectual property management and marketplace trading

*Aug 2023 - Dec 2023*

## 🚀 Overview

Nemo Markets IP CRM was a venture-backed startup that developed an AI-powered customer relationship management system specifically designed for intellectual property management. The platform featured a marketplace where organizations could list and trade IP assets, providing a comprehensive solution for IP portfolio management.

**[Live Demo](https://shorturl.at/LYztf)**

## 🏗️ Project Structure

This is a full-stack application with separate frontend and backend directories:

```
nemo-markets-ip-crm/
├── backend/          # Fastify API server
│   ├── server.ts     # Main server logic
│   ├── utils/        # Utility functions
│   └── ...
├── frontend/         # Next.js React application
│   ├── app/          # Next.js app router
│   ├── components/   # React components
│   └── ...
└── README.md
```

## 📋 Features

### Portfolio Management
- Create, update, and delete IP assets
- Organize assets by category, stage, and description
- Set asking prices for asset valuation
- Track portfolio metrics and analytics

### Marketplace
- List portfolios for public trading
- Browse available IP portfolios
- Filter by sector, status, and asset types
- View detailed portfolio information including:
  - Company information and background
  - Asset composition and pricing
  - Investor information
  - Key performance metrics

### Asset Management
- Comprehensive asset categorization
- Stage-based asset tracking
- Dynamic pricing calculations
- Portfolio-level listing controls

## 🛠️ Tech Stack

**Frontend:**
- React.js
- Next.js 14+ (App Router)
- TypeScript
- Tailwind CSS
- Next/font optimization

**Backend:**
- Node.js
- Fastify
- TypeScript
- Prisma ORM

**Database:**
- PostgreSQL

**Runtime:**
- Node.js

## 🚀 Getting Started

### Prerequisites
- Node.js (v18+)
- PostgreSQL database

### Installation

1. Clone the repository
```bash
git clone [repository-url]
cd nemo-markets-ip-crm
```

2. Set up the Backend
```bash
cd backend
npm install

# Set up environment variables
cp .env.example .env
# Configure your database connection and other settings

# Initialize the database
npx prisma generate
npx prisma db push
```

3. Set up the Frontend
```bash
cd ../frontend
npm install
```

### Running the Application

1. Start the Backend Server (from `/backend` directory):
```bash
npm run dev
```
The API will be available at `http://localhost:4000`

2. Start the Frontend Development Server (from `/frontend` directory):
```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

## 🔧 API Endpoints

### Portfolio Management
- `GET /portfolio/:portfolio_unique_id` - Retrieve portfolio details
- `GET /marketplace` - List all available portfolios

### Asset Management
- `POST /vault/asset` - Create new asset
- `PATCH /vault/asset` - Update existing asset
- `DELETE /vault/asset` - Delete asset

### Market Operations
- `PATCH /vault/market-status` - Update portfolio listing status

## 📊 Data Models

### Portfolio
- Unique portfolio identifier
- Organization details and metrics
- Asset relationships
- Market listing status
- Display configuration

### Assets
- Asset categorization and staging
- Pricing information
- Portfolio associations
- Descriptive metadata

### Organization
- Company information
- Investor relationships
- Sector classification
- Operational status

## 🎨 Frontend Features

- **Font Optimization**: Uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font
- **App Router**: Built with Next.js 14+ App Router for enhanced performance
- **Responsive Design**: Tailwind CSS for modern, responsive UI
- **TypeScript**: Full type safety across the application

## 📚 Learn More

To learn more about the technologies used:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial
- [Fastify Documentation](https://www.fastify.io/docs/) - learn about the backend framework
- [Prisma Documentation](https://www.prisma.io/docs/) - database toolkit and ORM

## 🚀 Deployment

### Frontend Deployment
The easiest way to deploy the Next.js frontend is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out the [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

### Backend Deployment
The Fastify backend can be deployed to various platforms:
- Railway
- Heroku
- DigitalOcean App Platform
- AWS/GCP/Azure

## 🎯 Business Model

Nemo Markets operated as a B2B SaaS platform targeting:
- IP management firms
- Technology companies with substantial patent portfolios
- Investment firms specializing in intellectual property
- Legal firms handling IP transactions

## 📈 Key Learnings

This project provided valuable insights into:
- **Founder-Market Fit**: The importance of deep domain expertise in specialized markets
- **Full-Stack Development**: Building cohesive frontend and backend systems
- **B2B SaaS Complexity**: The challenges of building enterprise-grade IP management tools
- **Market Validation**: The critical need for extensive customer discovery in niche markets
- **Technical Architecture**: Building scalable systems for complex data relationships

## 🏁 Project Status

**Status: Wound Down (Dec 2023)**

After recognizing founder-market misalignment and conducting thorough market analysis, the decision was made to wind down operations. This experience provided invaluable lessons for future entrepreneurial ventures.

The codebase serves as a comprehensive example of:
- Modern full-stack TypeScript development
- Next.js best practices with App Router
- Fastify API development with Prisma
- Enterprise-level application architecture

## 🛡️ Security & Compliance

- CORS implementation for secure cross-origin requests
- Input validation and sanitization
- Database query optimization with Prisma
- Environment-based configuration management
- Type-safe API communication between frontend and backend

## 📝 License

This project was developed as a commercial venture. Code samples provided for demonstration purposes.

---

*Built with ❤️ and lessons learned for future ventures*

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - feedback and contributions are welcome!
