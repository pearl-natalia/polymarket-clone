# Polymarket Clone - Database Setup Guide

## Project Overview
Prediction Market Platform (Milestone 0)  
Team: Akshar Barot, Darsh Shah, Krish Modi, Pearl Natalia, Sanskriti Akhoury  
Course: CS 348 - Database Systems  

## Technology Stack
- **Database**: PostgreSQL hosted on Supabase  
- **Application**: Next.js with React frontend  
- **Development**: Local machines with VS Code Live Share  
- **Deployment**: Vercel (frontend) + Supabase (database)  

## Database Platform Choice

As outlined in our Milestone 0 report, we selected PostgreSQL on Supabase for our managed database solution. This choice provides:

- Cloud-hosted PostgreSQL with automatic backups
- Real-time database features for dynamic updates
- Built-in authentication integration
- Seamless integration with Next.js applications
- Automatic scaling and performance optimization

## Sample Database Structure

Our toy database consists of three core tables for initial development:

### 1. Users Table
- Stores basic user account information
- Fields: username, email, account balance, registration date
- Supports basic authentication and profile management

### 2. Markets Table  
- Contains prediction market information
- Fields: title, category, status, creation date
- Categories include politics, sports, crypto, entertainment

### 3. Bids Table
- Records user predictions on market outcomes
- Fields: user reference, market reference, outcome (YES/NO), amount
- Demonstrates basic trading functionality

## Database Setup Process

1. **Supabase Project Creation**
   - Create new project through Supabase dashboard
   - Configure PostgreSQL instance with team access

2. **Schema Implementation**
   - Create tables with proper relationships
   - Implement foreign key constraints
   - Add basic data validation rules

3. **Sample Data Loading**
   - Insert test users with varying balances
   - Create sample markets across different categories
   - Add initial bids to demonstrate trading

4. **Connection Configuration**
   - Set up environment variables for secure access
   - Configure Next.js API routes for database connectivity
   - Test basic CRUD operations

## Sample Dataset

Our toy dataset includes:

- **Users**: 3-5 test accounts with different balance levels
- **Markets**: 4-6 prediction markets covering:
  * "Will Bitcoin reach $100K by 2025?" (Crypto)
  * "Will it rain in Waterloo tomorrow?" (Weather) 
  * "Will the Raptors make playoffs?" (Sports)
  * "Who will win the next election?" (Politics)
- **Bids**: 8-10 sample bids across different markets and outcomes

## Testing and Verification

- Simple Next.js API route for database connectivity testing
- Basic SELECT queries to verify data retrieval
- Frontend test page to display database results
- Error handling for connection issues

## Team Development Setup

- Shared Supabase project with team member access
- GitHub repository with organized file structure
- Environment configuration for local development
- Documentation for setup and troubleshooting

## Security Considerations

- Database credentials stored in environment variables
- No sensitive information committed to version control
- Team access managed through Supabase dashboard
- API routes secured with proper authentication

## Future Expansion (Milestone 1+)

This basic setup provides the foundation for:
- Enhanced schema with complex relationships
- User portfolio tracking and transaction history
- Market price history and analytics
- Administrative tools for market management
- Advanced trading functionality

## Repository Information

Project repository: https://github.com/pearl-natalia/polymarket-clone

The repository contains:
- Next.js application structure
- Database schema definitions
- API route implementations  
- Sample data generation scripts
- Comprehensive setup documentation

## Support and Troubleshooting

For setup issues or questions:
1. Check Supabase dashboard for database status
2. Verify environment variable configuration
3. Review API route implementation
4. Consult team members or course TAs

This toy database setup demonstrates the core database connectivity and CRUD operations required for Milestone 0 while providing a solid foundation for future development milestones.
