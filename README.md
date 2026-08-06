# Mahadasara Auction Arena

A comprehensive sports auction platform built for Mahadasara College Sports, designed to manage player auctions, team bidding, and franchise management in an interactive and user-friendly interface.

## 🏆 Overview

The Mahadasara Auction Arena is a modern web application that facilitates sports player auctions for college teams. It provides a complete auction management system with real-time bidding, player showcase, team dashboard, and comprehensive administrative features for managing players and franchises.

## ✨ Features

### Core Auction Functionality
- **Live Auction System**: Real-time bidding with increment controls
- **Player Showcase**: Display current player up for auction with detailed information
- **Team Dashboard**: View all participating teams with their purse status and player count
- **Auction Controls**: Complete control over auction flow (Sell, Unsold, Next, Undo, Reset)
- **Bid History**: Track all auction activities with timestamps and detailed logs

### Player Management
- **Player Registration**: Add new players with images, positions, and base prices
- **Player Profiles**: Detailed player information including skills and statistics
- **Position Categories**: Batsman, Bowler, All-Rounder, Wicket-Keeper, Captain
- **Status Tracking**: Track player status (Available, Sold, Unsold)
- **Image Upload**: Upload player photos with intuitive image uploader

### Franchise Management
- **Team Registration**: Add and manage participating franchises
- **Purse Management**: Track team budgets and remaining funds
- **Team Logos**: Upload team logos for visual identification
- **Player Assignment**: Automatically assign sold players to respective teams
- **Financial Tracking**: Monitor spending and remaining budget for each team

### User Interface
- **Modern Design**: Dark-themed professional interface with auction-themed colors
- **Responsive Layout**: Works seamlessly on desktop and mobile devices
- **Real-time Updates**: Live updates of bids, auction status, and team purses
- **Filtering System**: Filter players by status, position, and availability
- **Toast Notifications**: User-friendly notifications for all actions

## 🛠️ Technology Stack

### Frontend Framework
- **React 18.3.1**: Modern React with hooks and functional components
- **TypeScript 5.5.3**: Type-safe development with full TypeScript support
- **Vite 5.4.1**: Fast build tool and development server

### UI Components & Styling
- **Tailwind CSS 3.4.11**: Utility-first CSS framework
- **shadcn/ui**: Comprehensive component library built on Radix UI
- **Radix UI**: Accessible, unstyled component primitives
- **Lucide React**: Beautiful icon library
- **Tailwind Animate**: Animation utilities for Tailwind CSS

### State Management & Data
- **React Context API**: Global state management for auction state
- **React Hook Form 7.53.0**: Form handling with validation
- **Zod 3.23.8**: Schema validation
- **TanStack React Query 5.56.2**: Data fetching and caching
- **UUID 11.1.0**: Unique identifier generation

### Routing & Navigation
- **React Router DOM 6.26.2**: Client-side routing
- **Browser Router**: Hash-based routing for SPA navigation

### Utilities & Helpers
- **date-fns 4.1.0**: Date formatting and manipulation
- **clsx 2.1.1**: Conditional className utility
- **tailwind-merge 2.5.2**: Merge Tailwind CSS classes intelligently
- **class-variance-authority 0.7.1**: Component variant management

### Development Tools
- **ESLint 9.9.0**: Code linting and quality checks
- **TypeScript ESLint 8.0.1**: TypeScript-specific linting rules
- **PostCSS 8.4.47**: CSS transformation
- **Autoprefixer 10.4.20**: CSS vendor prefixing

## 📁 Project Structure

```
mahadasara-auction-arena/
├── public/                      # Static assets
│   ├── favicon.ico             # Site favicon
│   ├── placeholder.svg         # Default placeholder image
│   └── robots.txt              # SEO robots file
├── src/
│   ├── components/             # React components
│   │   ├── ui/                 # shadcn/ui components (50+ components)
│   │   │   ├── accordion.tsx
│   │   │   ├── alert-dialog.tsx
│   │   │   ├── alert.tsx
│   │   │   ├── aspect-ratio.tsx
│   │   │   ├── avatar.tsx
│   │   │   ├── badge.tsx
│   │   │   ├── breadcrumb.tsx
│   │   │   ├── button.tsx
│   │   │   ├── calendar.tsx
│   │   │   ├── card.tsx
│   │   │   ├── carousel.tsx
│   │   │   ├── chart.tsx
│   │   │   ├── checkbox.tsx
│   │   │   ├── collapsible.tsx
│   │   │   ├── command.tsx
│   │   │   ├── context-menu.tsx
│   │   │   ├── dialog.tsx
│   │   │   ├── drawer.tsx
│   │   │   ├── dropdown-menu.tsx
│   │   │   ├── form.tsx
│   │   │   ├── hover-card.tsx
│   │   │   ├── input-otp.tsx
│   │   │   ├── input.tsx
│   │   │   ├── label.tsx
│   │   │   ├── menubar.tsx
│   │   │   ├── navigation-menu.tsx
│   │   │   ├── pagination.tsx
│   │   │   ├── popover.tsx
│   │   │   ├── progress.tsx
│   │   │   ├── radio-group.tsx
│   │   │   ├── resizable.tsx
│   │   │   ├── scroll-area.tsx
│   │   │   ├── select.tsx
│   │   │   ├── separator.tsx
│   │   │   ├── sheet.tsx
│   │   │   ├── sidebar.tsx
│   │   │   ├── skeleton.tsx
│   │   │   ├── slider.tsx
│   │   │   ├── sonner.tsx
│   │   │   ├── switch.tsx
│   │   │   ├── table.tsx
│   │   │   ├── tabs.tsx
│   │   │   ├── textarea.tsx
│   │   │   ├── toast.tsx
│   │   │   ├── toaster.tsx
│   │   │   ├── toggle-group.tsx
│   │   │   ├── toggle.tsx
│   │   │   ├── tooltip.tsx
│   │   │   └── use-toast.ts
│   │   ├── AuctionControls.tsx   # Auction control buttons
│   │   ├── AuctionHistory.tsx    # Bid history display
│   │   ├── Header.tsx            # Application header
│   │   ├── ImageUploader.tsx     # Image upload component
│   │   ├── PlayerForm.tsx        # Player creation/editing form
│   │   ├── PlayerShowcase.tsx   # Current player display
│   │   ├── PlayersList.tsx       # Players list with filtering
│   │   ├── TeamDashboard.tsx     # Team overview cards
│   │   └── TeamForm.tsx          # Team creation/editing form
│   ├── context/                  # React Context providers
│   │   └── AuctionContext.tsx    # Global auction state management
│   ├── data/                     # Mock data and constants
│   │   └── mockData.ts          # Sample players, teams, and history
│   ├── hooks/                    # Custom React hooks
│   │   ├── use-mobile.tsx       # Mobile device detection
│   │   └── use-toast.ts         # Toast notification hook
│   ├── lib/                      # Utility functions
│   │   └── utils.ts             # className utility function
│   ├── pages/                    # Page components
│   │   ├── Index.tsx            # Main auction page
│   │   ├── ManageFranchises.tsx # Franchise management page
│   │   ├── ManagePlayers.tsx    # Player management page
│   │   └── NotFound.tsx         # 404 error page
│   ├── types/                    # TypeScript type definitions
│   │   └── auction.ts           # Auction-related types
│   ├── App.tsx                   # Main application component
│   ├── App.css                   # Application-specific styles
│   ├── index.css                 # Global styles and Tailwind imports
│   ├── main.tsx                  # Application entry point
│   └── vite-env.d.ts            # Vite type definitions
├── .git/                        # Git repository
├── .gitignore                   # Git ignore rules
├── components.json              # shadcn/ui component configuration
├── eslint.config.js             # ESLint configuration
├── index.html                   # HTML entry point
├── package.json                 # Project dependencies and scripts
├── package-lock.json            # Dependency lock file
├── postcss.config.js            # PostCSS configuration
├── tailwind.config.ts           # Tailwind CSS configuration
├── tsconfig.json                # TypeScript configuration
├── tsconfig.app.json            # App TypeScript configuration
├── tsconfig.node.json           # Node TypeScript configuration
└── vite.config.ts               # Vite build configuration
```

## 🚀 Getting Started

### Prerequisites
- Node.js 18.x or higher
- npm, yarn, or bun package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/rishanmenezes/Mahadasara-Auction-Arena.git
   cd Mahadasara-Auction-Arena
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   # or
   bun install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   # or
   bun dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:8080` to view the application

### Available Scripts

- `npm run dev` - Start development server with hot reload
- `npm run build` - Build for production
- `npm run build:dev` - Build for development mode
- `npm run lint` - Run ESLint for code quality checks
- `npm run preview` - Preview production build locally

## 🎯 Application Pages

### Main Auction Page (`/`)
The primary auction interface featuring:
- **Player Showcase**: Large display of current player with image, name, position, and pricing
- **Auction Controls**: Control buttons for Sell, Unsold, Next, Undo, and Reset
- **Team Dashboard**: Grid of all franchise teams with purse information
- **Players List**: Comprehensive list of all players with filtering options
- **Auction History**: Real-time activity feed of all auction events

### Manage Players (`/manage-players`)
Player administration interface with:
- **Search Functionality**: Find players by name or position
- **Add New Players**: Create player profiles with images and details
- **Edit Players**: Modify existing player information
- **Delete Players**: Remove players from the auction pool
- **Status Indicators**: Visual indicators for sold/available players

### Manage Franchises (`/manage-franchises`)
Team management interface with:
- **Search Functionality**: Find franchises by name
- **Add New Teams**: Create new franchises with logos and budgets
- **Edit Teams**: Modify team information and purse
- **Delete Teams**: Remove franchises from the auction
- **Financial Overview**: View initial and remaining purse for each team

## 🎨 Design System

### Color Palette
- **Primary Dark**: `#1A1F2C` - Main background color
- **Secondary (Gold)**: `#F59E0B` - Accents and highlights
- **Accent (Indigo)**: `#4F46E5` - Interactive elements
- **Highlight (Green)**: `#10B981` - Success states
- **Danger (Red)**: `#EF4444` - Error and destructive actions
- **Light**: `#F3F4F6` - Light backgrounds
- **Dark**: `#111827` - Dark backgrounds

### Typography
- Modern sans-serif font stack
- Responsive font sizes
- Clear hierarchy with proper weight variations

### Components
- Custom button styles (Primary, Secondary, Danger, Success)
- Card-based layouts with consistent styling
- Responsive grid systems
- Interactive hover states and transitions

## 📊 Data Models

### Player
```typescript
{
  id: string;
  name: string;
  imageUrl: string;
  basePrice: number;
  position: 'Batsman' | 'Bowler' | 'All-Rounder' | 'Wicket-Keeper' | 'Captain';
  skills: string[];
  stats: {
    battingAverage?: number;
    bowlingAverage?: number;
    matchesPlayed?: number;
    runsScored?: number;
    wicketsTaken?: number;
  };
  sold: boolean;
  soldTo?: string;
  soldAmount?: number;
}
```

### Team
```typescript
{
  id: string;
  name: string;
  logoUrl: string;
  color: string;
  initialPurse: number;
  remainingPurse: number;
  players: Player[];
}
```

### Auction State
```typescript
{
  currentPlayerId: string | null;
  currentBidAmount: number;
  currentBidTeamId: string | null;
  isAuctionInProgress: boolean;
  history: AuctionHistoryItem[];
}
```

## 🔧 Configuration

### Vite Configuration
- Development server on port 8080
- Path aliases for `@` pointing to `./src`
- React SWC plugin for fast refresh
- Component tagger for development mode

### TypeScript Configuration
- Strict mode disabled for flexibility
- Path aliases configured
- No implicit any disabled
- Allow JS for compatibility

### Tailwind Configuration
- Dark mode support
- Custom auction color palette
- Custom animations (pulse-bid, fade-in)
- Responsive breakpoints
- Container utilities

## 🎮 Usage Guide

### Starting an Auction
1. Navigate to the main auction page
2. Select a player from the Players List
3. Click "Auction" button next to the player
4. The player appears in the Player Showcase
5. Teams can now place bids using the "Place Bid" buttons

### Placing Bids
1. Ensure auction is in progress
2. Click "Place Bid" on the desired team card
3. Bids increment by ₹500 automatically
4. Current bid amount updates in real-time
5. Bid history records each bid with timestamp

### Selling Players
1. Place at least one bid on the current player
2. Click "Sell" in the Auction Controls
3. Player is assigned to the winning team
4. Team purse is reduced by the final bid amount
5. Player status changes to "Sold"

### Managing Players
1. Navigate to "Manage Players" page
2. Use search to find specific players
3. Click "Add New Player" to create new entries
4. Edit existing players with the pencil icon
5. Delete players using the trash icon (if not sold)

### Managing Franchises
1. Navigate to "Manage Franchises" page
2. Click "Add New Franchise" to create teams
3. Set team name and initial purse
4. Upload team logo for visual identification
5. Edit or delete franchises as needed

## 🔄 State Management

The application uses React Context API for global state management:

### AuctionContext
- **Players State**: Array of all players with their current status
- **Teams State**: Array of all franchises with purse information
- **Auction State**: Current auction progress and bidding information
- **Actions**: Start auction, place bid, sell player, mark unsold, undo, reset

### Reducer Pattern
Auction state is managed using a reducer pattern with the following actions:
- `START_AUCTION`: Begin auction for a specific player
- `PLACE_BID`: Record a team bid with amount
- `SELL_PLAYER`: Complete player sale to winning team
- `MARK_UNSOLD`: Mark player as unsold
- `NEXT_PLAYER`: Move to next player
- `UNDO_LAST_ACTION`: Revert most recent action
- `RESET_AUCTION`: Reset entire auction state

## 🧪 Testing & Development

### Code Quality
- ESLint configuration for consistent code style
- TypeScript for type safety
- React Hook Form for form validation
- Zod schemas for data validation

### Development Features
- Hot Module Replacement (HMR) for fast development
- Component tagger for development debugging
- Source maps for easy debugging
- Responsive design testing tools

## 📱 Responsive Design

The application is fully responsive with:
- Mobile-first approach
- Adaptive layouts for different screen sizes
- Touch-friendly interface elements
- Optimized viewing for tablets and desktops

## 🔐 Security Considerations

- Client-side validation using Zod schemas
- Input sanitization for user-provided data
- Image upload restrictions to image files only
- Protected actions (sold players cannot be deleted)

## 🚀 Deployment

### Build for Production
```bash
npm run build
```

### Preview Production Build
```bash
npm run preview
```

### Deployment Platforms
The application can be deployed to:
- Vercel
- Netlify
- GitHub Pages
- Any static hosting service

## 🤝 Contributing

Contributions are welcome! Please follow these guidelines:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is part of Mahadasara College Sports and is intended for educational and institutional use.

## 👥 Authors

- **Rishan Menezes** - Project Lead & Developer

## 🙏 Acknowledgments

- Mahadasara College Sports Department
- shadcn/ui for the excellent component library
- Radix UI for accessible component primitives
- The React and TypeScript communities

## 📞 Support

For support, questions, or feedback:
- GitHub Issues: [Project Issues](https://github.com/rishanmenezes/Mahadasara-Auction-Arena/issues)
- Contact: Through GitHub repository

---

**Built with ❤️ for Mahadasara College Sports**
