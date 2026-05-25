Core Financial Logic
Income Management: Accepts primary income with automated numerical formatting.
Fixed Expense Tracking: Pre-configured with "Rent" and "Utilities" to establish a baseline for recurring monthly costs.
Dynamic Variable Expenses: Includes a UI-driven function to add an unlimited number of custom variable expenses (e.g., "Subscriptions," "Fuel") on the fly.
Real-time Budget Calculation: Automatically computes the monthly surplus or deficit by subtracting total fixed and variable expenses from the primary income.
Holiday Planning & Goal Setting
Dedicated Holiday Expenses: Tracks specific travel-related costs (Tickets/Gas, Hotel/Camping, Food, Entertainment).
Savings Timeline Calculator: Automatically calculates the number of months required to fund the holiday based on the user's current monthly surplus
Multi-Currency Conversion:
Fetches live exchange rates using an external API (exchangerate-api.com).
Allows the user to select one base currency and two secondary currencies to view total costs in different global denominations simultaneously.
User Experience (UX) & Interface (UI)
Reactive Design (Real-time Updates): Utilizes onblur event listeners, meaning the calculator automatically refreshes all calculations and formatting the moment a user finishes typing in a field, eliminating the need to click a "Calculate" button constantly.
Dynamic UI Feedback:
Color-coded Alerts: The result box changes color dynamically—Red for a deficit (warning the user to adjust expenses), Yellow for breaking even, and Green for a positive surplus (encouraging the user).
Professional Formatting: * Forces thousands separators (commas) for readability.
Strict currency symbol application based on the user's selected region.
Responsive Layout: Built with Tailwind CSS, the interface automatically adjusts its layout to look professional on mobile phones, tablets, and desktop computers.
Technical Implementation (For your CS assignment)
Asynchronous JavaScript: Employs async/await patterns to fetch data from the exchange rate API, ensuring the UI doesn't "freeze" while waiting for the data.
DOM Manipulation: Uses standard JavaScript to programmatically inject new HTML elements into the DOM, allowing users to add expense rows dynamically.
calability: The code uses class-based selectors (fixed-exp, var-exp, hol-exp), making it easy to add more features or expense categories later without rewriting the core calculation logic.
Suggested Feature Summary for your Documentation:
The Budget & Holiday Planner is a full-stack, client-side web application.
It features real-time financial data processing, dynamic DOM manipulation for customizable budget line items, nd asynchronous API integration for global currency conversion, all wrapped in a responsive, accessible user interface.
