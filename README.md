# AI-Powered Exam Generator

This is a modern, AI-powered exam generation tool built with **Next.js**, **TailwindCSS**, and **Google Generative AI**. It allows educators to quickly generate exams based on user-defined parameters and export them with ease.

## Features

- **AI-Generated Questions**: Uses Google's Gen AI to dynamically create exam questions.
- **Export to Document**: Supports exporting generated exams into a document format.
- **Diagnostics Tool**: Helps verify the availability and status of required AI models.
- **Interactive UI**: Built with reusable and accessible components powered by ShadCN UI.

---

## Directory Structure

```bash
brayanj4y-ai-powered-exam-generator/
├── app/                      # Next.js app directory
│   ├── globals.css           # Global CSS
│   ├── layout.tsx           # App layout
│   ├── page.tsx             # Main landing page
│   └── api/                 # API route handlers
│       ├── check-models/
│       │   └── route.ts     # Endpoint to check model availability
│       └── export-exam/
│           └── route.ts     # Endpoint to export generated exams
│
├── components/              # React components
│   ├── *.tsx                # Main UI components
│   └── ui/                  # ShadCN-based UI components
│
├── hooks/                   # Custom hooks
│   ├── use-mobile.tsx
│   └── use-toast.ts
│
├── lib/                     # Utility functions and service clients
│   ├── check-models.ts
│   ├── document-generator.ts
│   ├── google-ai-client.ts
│   ├── question-generator.ts
│   └── utils.ts
│
├── styles/                  # Global styles
│   └── globals.css
│
├── public/                  # Static assets
├── tailwind.config.ts       # TailwindCSS configuration
├── postcss.config.js
├── tsconfig.json
├── next.config.js
├── package.json
├── pnpm-lock.yml
├── README.md
├── LICENSE
└── components.json
```
## Getting Started

**Prerequisites**

	•	Node.js >= 18
	•	Google Gen AI API key (for question generation)

**Installation**
```bash
npm install
```
**Development**
```bash
npm run dev
```
---
## Environment Variables

Create a ".env.local" file at the root and include:
```bash
GOOGLE_API_KEY=your_google_gen_ai_api_key
```
