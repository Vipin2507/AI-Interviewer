# Prepwise AI Mock Interviewer

Prepwise is an intelligent mock interview web application designed to help you get interview-ready through AI-powered practice and instant feedback. Built with Next.js and Firebase, Prepwise simulates real interview environments (like a live videocall with a recruiter), evaluates your responses, and provides comprehensive AI-driven feedback.

## Features

- **Live AI Interview Emulation:** Practice with natural voice conversations directly from your browser.
- **Customized Mock Inteviews:** Select roles, question types, and tech stacks to generate customized interview questions.
- **Real-Time Voice Feedback:** Uses Vapi AI and Google AI to process fast natural language conversations.
- **Comprehensive Feedback System:** Receive detailed AI reports on your performance and areas of improvements after each session.
- **Interview History:** Dashboard to manage and review past interviews inside your account. 
- **Modern UI:** Engaging interfaces heavily using Tailwind CSS, ShadCN UI and advanced client-components for a smooth user experience.

## Tech Stack

This project is built using modern web development tools:

- **Framework:** [Next.js 15](https://nextjs.org/) (React 19)
- **Styling:** [Tailwind CSS 4](https://tailwindcss.com/)
- **Authentication & Database:** [Firebase](https://firebase.google.com/)
- **Voice AI Processing:** [Vapi AI](https://vapi.ai/)
- **Text/NLP AI Processing:** [Google AI SDK](https://sdk.vercel.ai/providers/google)
- **Form Validation:** [React Hook Form](https://react-hook-form.com/) + [Zod](https://zod.dev/)

## Prerequisites

Before starting, ensure that you have standard web development environments ready:
- Node.js (v20+)
- NPM or PNPM
- A Firebase project setup (for user auth and databases).
- Tokens/Keys for Vapi AI and Google Gemini/AI SDK.

## Getting Started

Follow these instructions to set up your local development environment.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Vipin2507/AI-Interviewer.git
   cd prepwise
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up environment variables:**
   Create a `.env.local` file in the root directory and add the necessary environment variables required for Firebase and AI Providers:
   ```bash
   NEXT_PUBLIC_FIREBASE_API_KEY=""
   NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=""
   NEXT_PUBLIC_FIREBASE_PROJECT_ID=""
   NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=""
   NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=""
   NEXT_PUBLIC_FIREBASE_APP_ID=""

   NEXT_PUBLIC_VAPI_PUBLIC_KEY=""
   GOOGLE_AI_API_KEY=""
   ```

4. **Run the development server:**
   ```bash
   npm run dev
   ```

5. **Open the App:**
   Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Folder Structure

A brief overview of the top-level directory:

- `/app`: The core Next.js application including different page route components (`(auth)`, `(root)`, `api`).
- `/components`: Includes all React UI components (like `InterviewCard`, buttons, headers, and standard shadcn UI constructs).
- `/lib`: Helper models, constants, Actions and integration logic mapping (General App logic, AI operations, Auth Operations).
- `/firebase`: Firebase SDK clients and config initialization.
- `/public`: Static application assets (Robots icons, Favicons, etc).
- `/types`: Contains generic TypeScript type configurations used across the project logic.
- `package.json`: Main project configuration containing dependencies, scripts, and build info.

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.
