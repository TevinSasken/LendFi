# LendFi - Decentralized P2P Lending & ROSCA Platform

![LendFi Logo](https://via.placeholder.com/200x80/0ea5e9/ffffff?text=LendFi)

LendFi is a revolutionary peer-to-peer lending platform with ROSCA (Rotating Savings and Credit Association) features, built on Citrea ZK Rollup for secure Bitcoin transactions. The platform enables users to lend, borrow, and participate in collaborative savings groups with complete transparency and security.

## 🌟 Features

### Core Functionality
- **P2P Lending**: Direct lending between users with competitive rates
- **ROSCA Groups**: Rotating savings and credit associations for collaborative wealth building
- **Bitcoin Native**: All transactions use Bitcoin as the native currency through Citrea ZK Rollup
- **KYC Integration**: Secure identity verification for platform safety
- **Smart Contracts**: Automated, trustless transactions on Citrea blockchain

### User Features
- **Wallet Integration**: MetaMask and other Web3 wallet support
- **Loan Marketplace**: Browse and fund loan requests from verified borrowers
- **Personal Dashboard**: Track loans, ROSCA groups, and transaction history
- **Real-time Calculations**: Automatic interest and payment calculations
- **Mobile Responsive**: Optimized for all devices

### Admin Features
- **User Management**: KYC approval, user monitoring, and platform oversight
- **Loan Oversight**: Risk assessment, approval workflows, and default management
- **ROSCA Monitoring**: Group management and dispute resolution
- **Analytics Dashboard**: Platform health metrics and performance tracking

## 🚀 Technology Stack

### Frontend
- **React 19** with Vite for fast development
- **Tailwind CSS** for modern, responsive design
- **React Router** for client-side routing
- **React Hook Form** for form management
- **TanStack Query** for data fetching and caching
- **Lucide React** for beautiful icons

### Backend (Planned)
- **Node.js/Express** with TypeScript
- **PostgreSQL** with Sequelize ORM
- **JWT** for authentication
- **bcrypt** for password hashing
- **Helmet.js** for security

### Blockchain
- **Citrea ZK Rollup** (Type 2 zkEVM)
- **BitVM** for trust-minimized Bitcoin peg
- **Solidity** smart contracts
- **Web3.js** for blockchain interaction
- **Hardhat** for smart contract development

### Security & Compliance
- **KYC Integration** with Onfido API
- **AES-256** encryption for sensitive data
- **HTTPS** and security headers
- **Role-based access control**

## 📦 Installation

### Prerequisites
- Node.js v18 or higher
- npm or yarn package manager
- MetaMask or compatible Web3 wallet

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/lendfi.git
   cd lendfi
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173`

### Environment Setup

Create a `.env` file in the root directory:

```env
# Frontend Environment Variables
VITE_APP_NAME=LendFi
VITE_CITREA_RPC_URL=https://rpc.citrea.xyz
VITE_CITREA_CHAIN_ID=5115
VITE_ONFIDO_API_KEY=your_onfido_api_key

# Backend Environment Variables (when implemented)
DATABASE_URL=postgresql://username:password@localhost:5432/lendfi
JWT_SECRET=your_jwt_secret_key
ENCRYPTION_KEY=your_aes_256_key
ADMIN_SECRET=ADMIN_SECRET_2025
```

## 🎯 Usage Guide

### For Borrowers

1. **Register & Verify**
   - Create an account with email and password
   - Complete KYC verification with required documents
   - Connect your Web3 wallet

2. **Request a Loan**
   - Navigate to "Loan Request" page
   - Fill in loan details (amount, interest rate, duration, purpose)
   - Provide collateral description
   - Submit for marketplace listing

3. **Manage Your Loans**
   - Track loan status in "My Loans" section
   - Make repayments when loans are funded
   - View payment schedules and history

### For Lenders

1. **Browse Marketplace**
   - Explore available loan requests
   - Filter by amount, interest rate, duration, and purpose
   - Review borrower KYC status and ratings

2. **Fund Loans**
   - Select loans that match your criteria
   - Fund with one-click Bitcoin transactions
   - Track loan performance and repayments

### For ROSCA Participants

1. **Join or Create Groups**
   - Browse available ROSCA groups
   - Create new groups with custom parameters
   - Invite friends and community members

2. **Participate in Cycles**
   - Make regular contributions as scheduled
   - Receive payouts when it's your turn
   - Track group progress and member activity

### For Administrators

1. **User Management**
   - Review and approve KYC applications
   - Monitor user activity and compliance
   - Handle disputes and support requests

2. **Platform Oversight**
   - Monitor loan performance and defaults
   - Manage ROSCA group disputes
   - Configure platform settings and fees

## 🏗️ Project Structure

```
lendfi/
├── public/                 # Static assets
├── src/
│   ├── components/        # Reusable UI components
│   │   └── Layout/       # Header, Footer, Navigation
│   ├── contexts/         # React Context providers
│   │   └── AuthContext.jsx
│   ├── pages/            # Page components
│   │   ├── Home.jsx
│   │   ├── Auth.jsx
│   │   ├── Dashboard.jsx
│   │   ├── LoanRequest.jsx
│   │   ├── LoanMarketplace.jsx
│   │   ├── Loans.jsx
│   │   ├── ROSCA.jsx
│   │   ├── Transactions.jsx
│   │   └── AdminPanel.jsx
│   ├── hooks/            # Custom React hooks
│   ├── utils/            # Utility functions
│   ├── styles/           # Global styles and Tailwind config
│   ├── App.jsx           # Main application component
│   └── main.jsx          # Application entry point
├── contracts/            # Smart contracts (planned)
├── server/              # Backend API (planned)
├── docs/                # Documentation
└── tests/               # Test files
```

## 🔧 Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

### Code Style

The project uses:
- ESLint for code linting
- Prettier for code formatting
- Conventional commits for git messages

### Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 🔐 Security

### Current Security Measures
- Client-side form validation
- Secure password requirements
- Role-based access control
- KYC verification requirements
- Wallet signature verification (planned)

### Planned Security Enhancements
- Smart contract audits
- Penetration testing
- Bug bounty program
- Multi-signature wallets
- Insurance coverage

## 🚧 Roadmap

### Phase 1: MVP (Current)
- [x] User authentication and KYC
- [x] Loan request and marketplace
- [x] ROSCA group creation and management
- [x] Transaction history
- [x] Admin panel
- [x] Responsive UI/UX

### Phase 2: Blockchain Integration
- [ ] Citrea testnet deployment
- [ ] Smart contract development
- [ ] Wallet integration
- [ ] On-chain transactions
- [ ] BitVM implementation

### Phase 3: Advanced Features
- [ ] Credit scoring system
- [ ] Insurance integration
- [ ] Mobile app development
- [ ] API for third-party integrations
- [ ] Advanced analytics

### Phase 4: Scale & Optimize
- [ ] Mainnet deployment
- [ ] Performance optimization
- [ ] Global expansion
- [ ] Institutional features
- [ ] DeFi protocol integrations

## 📊 Platform Statistics

### Current Metrics (Demo Data)
- **Total Users**: 2,456
- **Verified Users**: 2,089 (85% approval rate)
- **Total Loans Funded**: ₿1,234.56
- **Active ROSCA Groups**: 89
- **Platform Success Rate**: 98.5%
- **Average Loan Size**: ₿0.025
- **Average Interest Rate**: 5.8%

## 🤝 Community

### Support Channels
- **Discord**: [Join our community](https://discord.gg/lendfi)
- **Telegram**: [LendFi Official](https://t.me/lendfi)
- **Twitter**: [@LendFiOfficial](https://twitter.com/lendfi)
- **Email**: support@lendfi.com

### Documentation
- [User Guide](./docs/user-guide.md)
- [Developer Documentation](./docs/developer-guide.md)
- [API Reference](./docs/api-reference.md)
- [Smart Contract Documentation](./docs/smart-contracts.md)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Citrea Labs** for the innovative ZK Rollup technology
- **Bitcoin Community** for the foundational blockchain infrastructure
- **Open Source Contributors** for the amazing tools and libraries
- **Early Users** for feedback and testing

## 📞 Contact

**LendFi Team**
- Website: [https://lendfi.com](https://lendfi.com)
- Email: team@lendfi.com
- LinkedIn: [LendFi Official](https://linkedin.com/company/lendfi)

---

**Built with ❤️ by the LendFi Team**

*Empowering financial inclusion through decentralized lending and collaborative savings.*