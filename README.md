# schwab-bot

A Discord bot for tracking stocks and managing watchlists using the Schwab API.

Features Authentication: Securely authenticate with Schwab API Stock Quotes: Get real-time stock quotes Watchlists: Create and manage stock watchlists Price Alerts: Set up price alerts for stocks Real-time Streaming: Stream real-time market data using Schwab's Streamer API Interactive Dashboards: Create real-time stock dashboards with automatic updates Enhanced Options Tracking: Monitor options contracts with real-time price updates, clear ITM/OTM/ATM indicators, and full chain navigation Paper Trading: Simulate real trading with virtual portfolios using real-time market data Comprehensive Help: Interactive help system with detailed command information Commands Help /help [command] - Get help with using the bot and its commands Authentication /auth login - Authenticate with Schwab API /auth logout - Log out from Schwab API /auth status - Check authentication status /auth code  - Complete authentication with a code
Stock Quotes
/quote  - Get a stock quote for a specific symbol
Watchlists
/watchlist create  [symbols] - Create a new watchlist
/watchlist list - List all your watchlists
/watchlist view  - View a specific watchlist
/watchlist add   - Add a symbol to a watchlist
/watchlist remove   - Remove a symbol from a watchlist
/watchlist delete  - Delete a watchlist
Price Alerts
/alert create     [options] - Create a new price alert
/alert multi     [options] - Create multiple price alerts at once
/alert delete  - Delete a price alert
/alert list - List all your price alerts
Real-time Streaming
/stream start   - Start streaming market data
/stream stop - Stop streaming market data
Dashboards
/dashboard create [symbols] [watchlist] [refresh] - Create a real-time dashboard with specified symbols or from a watchlist
/dashboard stop - Stop an active dashboard
Options
/options dashboard  [expiration] [type] [refresh] - Create a real-time options dashboard
/options stop - Stop an active options dashboard
Paper Trading
/trade portfolio - View your paper trading portfolio
/trade buy    [options] - Buy stocks or options with your paper trading account
/trade sell    [price] - Sell stocks or options from your paper trading account
/trade history [limit] - View your transaction history
/trade reset [balance] - Reset your paper trading portfolio
Dashboard Features
Real-time Updates: Prices update automatically via WebSocket streaming
Fallback Mechanism: Automatically falls back to REST API if streaming is unavailable
Interactive Controls: Refresh, add symbols, or stop the dashboard with buttons
Smart Data Handling: Intelligently merges data to prevent display of incomplete information
Multiple Symbol Support: Track up to 10 symbols simultaneously
Multiple Dashboards: Run multiple dashboards in different channels simultaneously (e.g., one for tech stocks, another for indices)
Channel-specific Views: Create dedicated dashboards for different market segments or watchlists

