# Patient Management System

A modern full-stack web application designed to streamline patient data handling for healthcare providers. Built with Next.js, TypeScript, and Tailwind CSS, the system allows efficient patient management with real-time SMS notifications via Twilio and backend services powered by Appwrite. The app also includes an admin panel with secure access and appointment control.

## 🧰 Tech Stack

- **Framework:** [Next.js](https://nextjs.org/)
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **Backend Services:** [Appwrite](https://appwrite.io/)
- **SMS Notifications:** [Twilio](https://www.twilio.com/)
- **Deployment:** [Vercel](https://vercel.com/)

## 🚀 Features

- ✅ **Patient Management:** Create, view, edit, and delete patient records.
- ✅ **SMS Notifications:** Send automatic messages via Twilio when appointments are scheduled or canceled.
- ✅ **Admin Panel:** Protected by passcode; view, approve, or cancel pending appointment requests.
- ✅ **Appwrite Integration:** Handles authentication, database operations, and secure data management.
- ✅ **Responsive UI:** Built with Tailwind CSS for desktop and mobile compatibility.
- ✅ **Modular Code:** Clean folder structure and reusable components.

## 🔐 Admin Panel

- Accessible only via a **secure Admin Passcode**.
- Displays all **pending appointment requests**.
- Admin can **schedule** or **cancel** appointments.
- Triggers **automated SMS notifications** to patients when actions are taken.

## 📦 Project Structure

```
├── app/                 # Application routes and pages
├── components/          # Reusable UI components
├── constants/           # Application constants
├── lib/                 # Utility libraries (e.g., Appwrite client, Twilio API)
├── public/              # Static assets (icons, images)
├── types/               # TypeScript types
├── .env.local           # Environment variables (not committed)
├── next.config.mjs      # Next.js configuration
├── tailwind.config.ts   # Tailwind configuration
└── README.md            # Project documentation
```

## 🛠️ Getting Started

### Prerequisites

- Node.js (v14 or later)
- npm or yarn
- Appwrite account + project
- Twilio account + phone number

### Installation

1. **Clone the repo**

```bash
git clone https://github.com/hafiz229/patient-management-system.git
cd patient-management-system
```

2. **Install dependencies**

```bash
npm install
# or
yarn install
```

3. **Configure environment variables**

Create a `.env.local` file in the root and add:

```env
NEXT_PUBLIC_APPWRITE_ENDPOINT=your_appwrite_endpoint
NEXT_PUBLIC_APPWRITE_PROJECT=your_project_id
APPWRITE_DATABASE_ID=your_database_id
TWILIO_ACCOUNT_SID=your_twilio_sid
TWILIO_AUTH_TOKEN=your_twilio_token
TWILIO_PHONE_NUMBER=your_twilio_phone
ADMIN_PASSCODE=your_secret_passcode
```

4. **Run the development server**

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## ⚙️ Deployment

Deployed using [Vercel](https://vercel.com/)

👉 **Live Demo:** [https://patient-management-system-hafiz-229.vercel.app](https://patient-management-system-hafiz-229.vercel.app)

To deploy your own:

- Connect your GitHub repo to Vercel.
- Add the environment variables in Vercel project settings.
- Deploy!

## 📄 License

This project is licensed under the [MIT License](LICENSE).

## 🙌 Acknowledgments

- [Next.js](https://nextjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Appwrite](https://appwrite.io/)
- [Twilio](https://www.twilio.com/)
- [Vercel](https://vercel.com/)