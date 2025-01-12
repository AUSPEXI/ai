# AI Tools Index

A comprehensive platform for discovering, comparing, and reviewing AI tools across different categories. Built with React, TypeScript, Tailwind CSS, and Supabase.

## Features

### Tool Discovery
- Search and filter AI tools by category, pricing type, and keywords
- Sort tools by rank, rating, or name
- Quick category filters for Text, Image, Audio, Video, and Business tools
- Detailed tool information including pricing, ratings, and descriptions

### Cost Calculator
- Calculate estimated costs based on usage duration
- Support for different pricing models (free, freemium, paid)
- Display minimum and maximum duration limits
- Show usage restrictions and limitations

### Special Offers
- View active promotional offers and discounts
- Exclusive deals with promo codes
- Time-limited offers with countdown
- Detailed terms and conditions

### Reviews & Ratings
- User reviews with ratings and detailed feedback
- Review moderation system
- Helpful/Report functionality for review quality
- Average ratings and review counts

### Analytics Dashboard
- Overview of key metrics
  - Total tools count
  - Number of categories
  - Average ratings
  - Active users
- Category distribution visualization
- Rating distribution by category
- Growth trends and popularity metrics

### User Management
- Email-based authentication
- User profiles
- Review management
- Secure authentication via Supabase

## Technical Architecture

### Frontend
- React 18.3 with TypeScript
- Tailwind CSS for styling
- Lucide React for icons
- Vite for development and building

### Backend
- Supabase for database and authentication
- PostgreSQL database with RLS policies
- Real-time subscriptions for live updates

### Database Schema

#### Tables
- `tools`: Main table for AI tool information
- `categories`: Tool categories
- `reviews`: User reviews and ratings
- `offers`: Special offers and promotions
- `tool_categories`: Junction table for tool-category relationships

## Getting Started

### Prerequisites
- Node.js 18+
- npm or yarn
- Supabase account

### Installation

1. Clone the repository:
\`\`\`bash
git clone [repository-url]
cd ai-tools-index
\`\`\`

2. Install dependencies:
\`\`\`bash
npm install
\`\`\`

3. Set up environment variables:
Create a \`.env\` file with your Supabase credentials:
\`\`\`
VITE_SUPABASE_URL=your-supabase-url
VITE_SUPABASE_ANON_KEY=your-supabase-anon-key
\`\`\`

4. Start the development server:
\`\`\`bash
npm run dev
\`\`\`

## Development

### Project Structure
\`\`\`
src/
├── components/        # React components
├── hooks/            # Custom React hooks
├── lib/              # Utilities and configurations
├── types/            # TypeScript type definitions
└── App.tsx           # Main application component
\`\`\`

### Key Components

#### AnalyticsDashboard
- Displays tool usage statistics
- Category distribution
- Rating analytics
- Growth trends

#### CostCalculator
- Calculates usage costs
- Handles different pricing models
- Shows usage limitations

#### ToolOffers
- Displays promotional offers
- Handles promo code copying
- Shows offer expiration

#### ReviewSystem
- User review submission
- Review display and moderation
- Rating calculations

### Custom Hooks

#### useAnalytics
- Fetches and processes analytics data
- Calculates statistics and trends
- Handles loading and error states

#### useTools
- Manages tool data fetching
- Handles filtering and sorting
- Supports search functionality

#### useReviews
- Manages review data
- Handles review submission
- Supports moderation features

#### useAuth
- Handles user authentication
- Manages user sessions
- Provides auth state

## Security

### Authentication
- Email-based authentication via Supabase
- Secure password handling
- Session management

### Database Security
- Row Level Security (RLS) policies
- Protected user data
- Secure API access

## Performance Optimization

### Data Fetching
- Efficient SQL queries
- Data pagination
- Caching strategies

### UI Performance
- React component optimization
- Lazy loading
- Efficient re-renders

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support, please open an issue in the repository or contact the maintainers.