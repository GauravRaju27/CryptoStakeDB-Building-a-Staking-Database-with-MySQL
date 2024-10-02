# CryptoStakeDB-Building-a-Staking-Database-with-MySQL
The Crypto Staking Database is a robust and scalable MySQL database designed to manage and facilitate crypto staking operations. This project includes multiple tables and triggers to handle user data, wallet management, staking packages, user memberships, ROI income, referrals, and rewards, making it a comprehensive solution for any crypto staking application.

Features
User Management: Handle user registration, authentication, and referral systems.
Wallet Management: Maintain user wallets with various income streams, including ROI and referral income.
Staking Packages: Define and manage staking packages with unique attributes such as amount and ROI.
Membership Management: Track user memberships and their associated staking packages.
Income Tracking: Automatically calculate and store ROI, referral, and level income.
Rewards System: Manage rewards for users based on their activity and business requirements.
Ledger Management: Keep track of wallet transactions, including opening and closing balances.

Database Structure
Tables
User: Stores user information including username, password, email, and referral codes.
Wallet: Manages user wallets and tracks available and reserved balances.
Packages: Defines staking packages available to users with details like ROI and duration.
User_Membership: Connects users to their selected packages and tracks membership details.
ROI_Income: Records ROI received by users from their investments.
UserReferral: Tracks referrals between users and their corresponding referral income.
Levels: Manages different levels of income based on user activity.
LevelIncome: Records income based on user levels and parent-child relationships among users.
Reward: Defines various rewards available to users.
User_Reward: Links users to their rewards, tracking when rewards are received.
Ledger: Maintains a transaction history for user wallets.

Triggers
Triggers are set up to automate actions, such as creating wallet entries for new users and updating wallet balances upon recording income and rewards.
User After Insert Trigger: Automatically creates a wallet entry for a new user upon registration.
ROI Income After Insert Trigger: Updates the wallet with the ROI income when it is recorded.
User Referral After Insert Trigger: Adds referral income to the wallet upon a new referral entry.
Level Income After Insert Trigger: Updates wallet records with level income upon insertion.
User Reward After Insert Trigger: Manages reward income updates in the wallet.

Getting Started:
To set up the database, clone the repository, create a MySQL database, and import the SQL scripts provided. The system allows for easy interaction through SQL queries, enabling the management of staking activities and user finances.
