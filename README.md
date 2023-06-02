## Introduction 👋

Next Portfolio is built using Next.js and Tailwind CSS for a modern design and rapid development. TypeScript is utilized for code clarity and safety. Additionally, Firebase is being integrated for backend services such as realtime-database. The result is a dynamic and functional portfolio website that showcases the developer's skills and experience.

## Tech Stack 🛠️

- [Next.js](https://nextjs.org)
- [TypeScript](https://www.typescriptlang.org)
- [Tailwind CSS](https://tailwindcss.com)
- [Firebase](https://firebase.google.com)
- [SendGrid](https://sendgrid.com)
- [Framer Motion](https://www.framer.com/motion)

## Development 💻

Here are the steps to run the portfolio locally.

1. Install dependencies

   ```bash
   npm i
   ```

2. Create a Firebase project and select the web app

3. Create an `.env.local` file in the root directory, and add the following variables with your firebase config:
   ```
   SENDGRID_API_KEY=XXXXXXXX
   NEXT_PUBLIC_FIREBASE_DATABASE_URL=XXXXXXXXXX
   MAIL_FROM=YOUR_MAIL_ID
   MAIL_TO=YOUR_MAIL_ID
   ```
   <!-- write text to tell user to get sendgrid keys from dashboard and add here -->

> **Note**: `SENDGRID_API_KEY` - Create an API key from "Settings" -> "API Keys" with "Restricted Access" to only "Mail Send"

4. Import json data

   - Go to [Firebase Console](https://console.firebase.google.com) and select your project
   - Go to "Database" -> "Realtime Database" -> "Import JSON" and import the [data.json] file

5. Run the project

   ```bash
   npm run dev
   ```

## Deployment 🚀

1. Create a Vercel account and select "Import Project"

2. Select the forked repository and deploy

3. Add the following environment variables in the Vercel dashboard:
   ```
   SENDGRID_API_KEY=XXXXXXXX
   NEXT_PUBLIC_FIREBASE_DATABASE_URL=XXXXXXXXXX
   MAIL_FROM=YOUR_MAIL_ID
   MAIL_TO=YOUR_MAIL_ID
   ```
4. Hurray! You successfully deployed the portfolio🥳
