# Expense Tracker

A beautiful and fully-featured React expense tracker application that helps you manage your personal finances with ease. Built with modern web technologies and designed for production use.

## Features

- **Transaction Management**: Add, view, and delete income and expense transactions
- **Real-time Balance**: Automatic calculation of total balance, income, and expenses
- **Category System**: Predefined categories for both income and expenses
- **Data Persistence**: All data is saved to localStorage and persists across browser sessions
- **Search & Filter**: Search transactions by description/category and filter by type
- **Sorting Options**: Sort transactions by date or amount


## Project Structure

```
src/
├── components/           # React components
│   ├── Summary.tsx      # Financial summary cards
│   ├── TransactionForm.tsx  # Add transaction form
│   └── TransactionList.tsx  # Transaction history and management
├── contexts/            # Context providers
│   └── ExpenseContext.tsx   # Main expense context with state management
├── hooks/               # Custom hooks
│   └── useLocalStorage.ts   # localStorage persistence hook
├── types/               # TypeScript type definitions
│   └── index.ts         # Transaction and context types
├── App.tsx             # Main application component
├── main.tsx            # Application entry point
└── index.css           # Global styles and Tailwind imports
```

## Getting Started

### Prerequisites
- Node.js (version 16 or higher)
- npm or yarn package manager

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd expense-tracker
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:5173`

### Building for Production

To create a production build:
```bash
npm run build
```

The built files will be in the `dist` directory.

## Customization

### Adding New Categories

To add new income or expense categories, edit the arrays in `src/types/index.ts`:

```typescript

export const INCOME_CATEGORIES = [
  'Salary',
  'Freelance',
];


