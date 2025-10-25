## 📱The Expenny 
Building a Full Stack Subscription Tracker. A real-time subscription tracking and analytics app with authentication and database storage.  

## 🎯Project Overview
Subscription Tracker is a full-stack web application designed to help users centrally manage and track all subscription services. Through an intuitive dashboard, users can view subscription expense statistics in real-time, manage subscription information, set reminders, and gain deep insights into their spending.

🎁 website : [https://main.d3qm9b2kfawktn.amplifyapp.com/](https://expennysubscriptiontracker.netlify.app/)

🌟Frontend:：Next.js
🌟Backend ：Firebase🔥 <b>（Authentication & Database）</b>
🌟Framwork:ReactJs
🌟Technology:Javascript, JSX, CSS, HTML
🌟Delopyment：Netlify


## 🌟 Core Features
1. User Authentication System

User registration and login functionality
Firebase Authentication for secure authentication
Automatic session management and logout
Real-time authentication state monitoring and synchronization

2. Subscription Management

Add Subscription: Quickly add new subscription services through forms
View Subscriptions: Display all subscriptions in a list format
Edit Subscriptions: Modify details of existing subscriptions
Delete Subscriptions: Remove unnecessary subscription records
Subscription information includes: service name, cost, billing cycle, next renewal date, etc.

3. Dashboard & Analytics

Subscription Overview: Quick view of subscription count and total expenses
Expense Analysis: Monthly and yearly cost breakdown
Categorized Display: Organize subscriptions by type
Real-time Updates: Subscription changes are immediately reflected on the dashboard

4. Responsive Design

Perfect adaptation to desktop, tablet, and mobile screens
Smooth user interface and interaction experience
Cross-device data synchronization

🛠️ Tech Stack
LayerTechnologyDetailsFrontend FrameworkNext.js + ReactModern Web Application DevelopmentProgramming LanguageJavaScript / JSXCore Development LanguageStylingCSS / HTMLInterface Design and LayoutState ManagementContext APIGlobal State Sharing and ManagementBackend ServiceFirebaseAuthentication & Realtime DatabaseDeploymentNetlifyCloud Hosting & Auto Deployment

## 💡 Core Implementation
1. Global State Management
Using Context API and useContext Hook to implement application-level state sharing:

Create AuthContext to manage authentication-related state
Create DataContext to manage user data and subscription information
Use Provider to wrap the entire application, enabling all components to access global state
Use useContext to access and update state in any component

State Content includes:

Authentication Info: login status, user ID, email
Business Data: subscription list, expense statistics, user preferences

2. Firebase Integration
Authentication

User Registration: Validate email and password, create Firebase user account
User Login: Verify credentials, generate session tokens
State Monitoring: Use onAuthStateChanged to listen for login state changes in real-time

Realtime Database

JSON-based NoSQL database
User Data Structure: User ID → Subscription Array → Subscription Objects
Real-time Sync: Database changes are instantly pushed to the frontend
Security Rules: Ensure users can only access their own data

3. Form Handling & Data Interaction
Form Management:

Use useState to manage form state
Handle form input with onChange events
Form validation and error messages
Submit event handling and data submission

Data Flow:

User enters information in form
onChange event triggers, updating local component state
User clicks submit button
Form data validation
Write data to Firebase
Firebase returns confirmation
Context updates global state
Component re-renders, showing latest data

4. Handler Functions

5. useEffect & Data Monitoring

Authentication Monitoring: Use useEffect + onAuthStateChanged to monitor user login state
Data Monitoring: Use useEffect + Firebase on() method to listen for database changes in real-time
Auto Re-render: Automatically trigger component re-render when data changes
Cleanup Functions: Properly clean up listeners when component unmounts to prevent memory leaks


This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
