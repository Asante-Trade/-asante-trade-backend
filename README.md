Asante Trade Backend

Backend API and core services powering the Asante Trade platform.

Overview

Asante Trade Backend is the central API and business logic layer for the Asante Trade ecosystem. It powers the platform's web dashboards, mobile applications, and future third-party integrations by providing secure, scalable services for authentication, agent management, customer operations, financial transactions, and blockchain connectivity.

Designed with financial inclusion in mind, the backend enables organizations to deliver digital financial services—including mobile wallets, remittances, savings, bill payments, and agent banking—to underserved communities across Africa.

The platform is being built with future integration into the Stellar blockchain and Soroban smart contracts to support fast, secure, and low-cost financial transactions.

Features
User Authentication & Authorization
Role-Based Access Control (Admin, Manager, Trainer, Agent, Customer)
Agent Management
Customer Management
KYC & AML Verification
Transaction Processing
Wallet Management
Savings Products
Bill Payments
Remittance Services
Notifications
Audit Logs
Reporting & Analytics APIs
Stellar Blockchain Integration (planned)
Soroban Smart Contract Integration (planned)
Tech Stack
Technology	Purpose
NestJS	Backend Framework
TypeScript	Programming Language
PostgreSQL	Primary Database
TypeORM	ORM
JWT	Authentication
Redis	Caching & Sessions (optional)
Swagger/OpenAPI	API Documentation
Docker	Containerization
Stellar SDK	Blockchain Integration (planned)
Soroban SDK	Smart Contract Integration (planned)
Project Structure
asante-trade-backend/
├── src/
│   ├── auth/
│   ├── users/
│   ├── agents/
│   ├── customers/
│   ├── transactions/
│   ├── wallets/
│   ├── kyc/
│   ├── notifications/
│   ├── reports/
│   ├── common/
│   ├── config/
│   └── main.ts
├── test/
├── docs/
├── .env.example
├── package.json
└── README.md

The structure above is illustrative. Modules may evolve as the project grows.

Getting Started
Prerequisites
Node.js 20+
PostgreSQL
npm, pnpm, or yarn
Installation
git clone https://github.com/Asante-Trade/asante-trade-backend.git

cd asante-trade-backend

npm install

or

pnpm install
Environment Variables

Create a .env file.

DATABASE_URL=

JWT_SECRET=

PORT=3001

STELLAR_NETWORK=testnet

STELLAR_RPC_URL=
Running the Application

Development

npm run start:dev

Production

npm run build

npm run start:prod
Available Scripts
npm run start

npm run start:dev

npm run build

npm run test

npm run lint

npm run format
API Documentation

Swagger documentation will be available after starting the server.

http://localhost:3001/api
Roadmap
Authentication & Authorization
Agent Management
Customer Management
Wallet Services
Transaction Engine
KYC/AML Verification
Bill Payments
Savings Products
Remittance Services
Notification Service
Reporting APIs
Stellar Integration
Soroban Smart Contracts
CI/CD Pipeline
Docker Deployment
Kubernetes Support
Security

Security vulnerabilities should be reported privately. Please do not open public issues for sensitive security reports.

Contributing

Contributions are welcome.

Before opening a pull request:

Check existing issues.
Open a discussion for major changes.
Follow the project's coding standards.
Write tests where applicable.

See CONTRIBUTING.md for contribution guidelines.

Related Repositories
Repository	Description
asante-trade-web	Web dashboards for administrators, managers, trainers, and customers
asante-trade-mobile (planned)	Agent mobile application
asante-trade-contracts (planned)	Soroban smart contracts
License

This project is licensed under the MIT License. See the LICENSE file for details.

Built to power accessible, secure, and scalable digital financial services across Africa through the Asante Trade ecosystem.