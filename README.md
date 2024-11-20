# Custom Email Sender

This repository contains the implementation of a custom email-sending application developed as part of the BreakoutAI Assessment. The application features a React-based frontend with capabilities to send personalized emails, track their delivery, and manage email schedules efficiently.

## Features

1. **Data Integration**:
   - Upload data via Google Sheets or CSV files for email customization.
   - Auto-detects columns for dynamic placeholder replacement in email templates.

2. **Email Account Integration**:
   - Supports connections via personal accounts (Gmail, Outlook) or SMTP/ESP integration using OAuth2.

3. **Customizable Prompt Box**:
   - Input email templates with placeholders (e.g., `{Company Name}`, `{Location}`) to personalize messages.

4. **Email Personalization & Sending**:
   - Generates custom email content using LLM APIs (e.g., Groq API).
   - Sends emails individually or in batches.

5. **Email Scheduling & Throttling**:
   - Schedule emails for specific times or stagger delivery intervals.
   - Configurable rate-limiting to respect provider limits.

6. **Real-Time Analytics**:
   - Dashboard displays total sent, pending, failed, and scheduled emails.
   - Tracks response rates and updates statuses in real-time.

7. **ESP Integration**:
   - Connect with providers like SendGrid, Amazon SES, or Mailgun for delivery tracking.
   - Supports tracking events like Delivered, Opened, Bounced, and Failed.

## Installation

### Prerequisites
- Node.js and npm installed.
- An ESP account (e.g., SendGrid, Mailgun) for email delivery tracking.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/custom-email-sender.git
   ```
2. Navigate to the project directory:
   ```bash
   cd custom-email-sender
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the development server:
   ```bash
   npm start
   ```

## Usage

1. **Data Input**:
   - Upload a CSV file or link a Google Sheet containing the necessary columns (e.g., Company Name, Email, Location).

2. **Customize Email**:
   - Use the prompt box to draft an email template with placeholders.

3. **Schedule Emails**:
   - Set a time for delivery or throttle the rate of email sending.

4. **Track Analytics**:
   - View delivery statuses, open rates, and failure counts on the dashboard.

## Deployment

- To deploy, build the app:
  ```bash
  npm run build
  ```
- Host the `build` folder on any static site hosting platform (e.g., Netlify, Vercel).

## Future Improvements

- Enhance dashboard UX with detailed charts.
- Add support for multi-language emails.
- Introduce advanced filtering and batch editing options.

## Contribution

Feel free to fork this repository and submit pull requests for enhancements. For major changes, please open an issue first.

## License

This project is licensed under the MIT License.
