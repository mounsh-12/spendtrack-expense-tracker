# SpendTrack – Personal Expense Tracker

SpendTrack is a full-stack personal expense tracking application that helps users manage their income and expenses in one place. It provides secure authentication, transaction management, balance tracking, and an administrative dashboard.

The application uses React for the frontend and AWS services for authentication, backend operations, and data storage.

## Features

- **User Authentication:** Secure user registration and login using Amazon Cognito.
- **Transaction Management:** Add, view, and delete financial transactions.
- **Income and Expense Tracking:** Manage income and expenses separately.
- **Category Management:** Organize transactions by category.
- **Balance Calculation:** Calculate available balance based on income and expenses.
- **Admin Dashboard:** Allow authorized administrators to view transaction data across users.
- **Cloud Backend:** Use AWS AppSync and GraphQL for backend communication.
- **Database Integration:** Store transaction data using Amazon DynamoDB.

## Technology Stack

| Category | Technologies |
|---|---|
| Frontend | React.js, JavaScript, HTML, CSS |
| Build Tool | Vite |
| Authentication | Amazon Cognito |
| API | AWS AppSync |
| API Query Language | GraphQL |
| Database | Amazon DynamoDB |
| Cloud Platform | Amazon Web Services |
| Version Control | Git, GitHub |

## Application Architecture

The application uses a cloud-based architecture.

1. Users interact with the application through the React frontend.
2. Amazon Cognito manages user authentication.
3. AWS AppSync handles GraphQL queries and mutations.
4. AWS Lambda can be used for backend processing where configured.
5. Amazon DynamoDB stores application transaction data.
6. Authorized administrators access the admin dashboard.

## Project Structure

```text
spendtrack/
│
├── public/
├── src/
│
├── app.jsx
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
├── eslint.config.js
├── .gitignore
└── README.md
```

*The structure is a simplified overview of the project.*

## Getting Started

Follow these steps to run SpendTrack locally.

### 1. Clone the Repository

```bash
git clone https://github.com/mounsh-12/spendtrack-expense-tracker.git
```

### 2. Navigate to the Project

```bash
cd spendtrack-expense-tracker
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Configure AWS Services

Configure the required AWS resources and application settings:

- Amazon Cognito
- AWS AppSync
- Amazon DynamoDB

Use your own AWS configuration. Do not upload AWS credentials, passwords, or private environment files to GitHub.

### 5. Start the Development Server

```bash
npm run dev
```

Open the local URL displayed in your terminal to access the application.

## Production Deployment

The frontend can be built for production using:

```bash
npm run build
```

The generated production files are placed in the `dist` directory.

The frontend can be hosted using Amazon S3 and delivered through Amazon CloudFront.

## Security

- User authentication is handled through Amazon Cognito.
- Administrative access should be restricted to authorized users.
- Environment variables and sensitive credentials must not be committed to GitHub.
- AWS permissions should follow the principle of least privilege.

## Future Enhancements

- Interactive financial analytics and charts.
- Monthly and yearly expense reports.
- Budget planning and alerts.
- Downloadable transaction reports.
- Docker containerization.
- CI/CD pipeline for automated deployment.
- Infrastructure as Code using Terraform.

## Author

**Mounish Reddy Sapparam**

GitHub: https://github.com/mounsh-12

Project Repository: https://github.com/mounsh-12/spendtrack-expense-tracker

---

**SpendTrack – Track your money. Understand your spending. Manage your finances.**
