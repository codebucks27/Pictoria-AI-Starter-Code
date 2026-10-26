# Pictoria AI - Personalized AI Photo Generation Platform

Transform your photos with the power of AI! Pictoria AI is your ultimate solution for creating/generating professional AI-generated photos, similar to the popular PhotoAI platform. Perfect for LinkedIn headshots, Instagram content, dating profile pictures, and professional portraits. Train AI model on your personal images and generate stunning, high-quality AI-generated photos within minutes.

This repository is the **tutorial starting scaffold**. Its current homepage is the initial Next.js page; the completed app's authentication, dashboard, AI, billing, and email integrations are built during the video. The features and screenshots below show that completed tutorial application.

![GitHub stars](https://img.shields.io/github/stars/codebucks27/Pictoria-AI-Starter-Code?style=social&logo=ApacheSpark&label=Stars)&nbsp;&nbsp;
![GitHub forks](https://img.shields.io/github/forks/codebucks27/Pictoria-AI-Starter-Code?style=social&logo=KashFlow&maxAge=3600)&nbsp;&nbsp;
![Github Followers](https://img.shields.io/github/followers/codebucks27.svg?style=social&label=Follow)&nbsp;&nbsp;<br />

If you want to learn how to create it please follow below tutorial👇: <br />
➡ Tutorial Link 💚: [How to Build a $1M PhotoAI Sass Clone](https://youtu.be/7AQNeii5K7E) <br />
➡ Final Source Code💛: [Pictoria-AI-Final](https://github.com/codebucks27/Pictoria-AI-Final)

The maintainer is preparing a free final-source release. As of 2026-10-26, the final repository is private; public access and a license decision are pending. Its existing purchaser-only license restricts redistribution, and source visibility alone does not grant open-source rights. You can follow the tutorial with this starter while those decisions are completed.


🎯 For customised solutions or deployment please contact: https://tally.so/r/wdlj0N


#### ⭐DO NOT FORGET TO STAR THIS REPO⭐

## 🚀 Completed Tutorial Features


- 🛠️ Complete SaaS built in modern Next.js
- 💻 Beautiful landing page included
- 🤖 Train AI model on your personal images
- 🖥️ Clean & intuitive event monitoring dashboard
- 🎯 AI-Powered Professional Photo Generation
- 🎨 Custom AI Model Training
- 💼 Professional LinkedIn Headshots
- 🌟 Clean, modern UI on top of shadcn-ui
- 📱 Social Media Content Generation
- 💳 Integrated Payment System
- ✉️ Email Notifications
- 📊 Usage Analytics
- 🎁 ...much more

## Images of The AI App:

These reference screenshots show the completed tutorial, rather than the current starter homepage.

![Photo AI clone Dashboard](https://github.com/codebucks27/Pictoria-AI-Starter-Code/blob/main/screenshots/Dashboard.png)
---
![Photo AI clone Image Generation Page](https://github.com/codebucks27/Pictoria-AI-Starter-Code/blob/main/screenshots/Image-Generation.png)
---
![Photo AI clone Model Training Page](https://github.com/codebucks27/Pictoria-AI-Starter-Code/blob/main/screenshots/Model-Training.png)
---
![Photo AI clone Billing Page](https://github.com/codebucks27/Pictoria-AI-Starter-Code/blob/main/screenshots/Billing.png)
---
![Photo AI clone Account Settings Page](https://github.com/codebucks27/Pictoria-AI-Starter-Code/blob/main/screenshots/Account-Settings.png)

## 🛠️ Tech Stack

- **Framework:** Next.js 15.2.3 (App Router), React 18
- **Styling:** Tailwind CSS 3
- **Language:** TypeScript
- **Dependency management:** npm, with `package-lock.json`

The video adds Shadcn UI, Supabase (PostgreSQL and Auth), Replicate, Stripe, and Resend. Their clients and application flows are not installed or implemented in this starter. The final repository has its own Node.js 24/Bun, Next.js 16, React 19, and Tailwind CSS 4 setup; use its instructions when working with that code.

## ⚡ Prerequisites

To run the scaffold, install Node.js and npm. This repository does not pin a Node.js version or package-manager version; choose a supported Node.js LTS environment compatible with its Next.js version.

To implement the service integrations while following the video, you will also need your own:

- A Supabase account
- A Replicate account
- A Stripe account
- A Resend account

## 🚀 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/codebucks27/Pictoria-AI-Starter-Code.git
cd Pictoria-AI-Starter-Code
```

### 2. Install Dependencies

```bash
npm ci
```

Use the checked-in `package-lock.json` for reproducible starter installs. Follow the final repository's Bun instructions separately if you have access to the completed source.

### 3. Environment Variables

No service credentials are required for the current scaffold homepage. When you implement integrations from the video, copy `.env.example` to a local `.env.local` and supply only your own development values. The starter template is tutorial reference material with legacy names; the final source has an updated template and setup guide. Never commit real credentials or expose privileged service keys through `NEXT_PUBLIC_` variables.

### 4. Supabase Tutorial Reference

The scaffold does not connect to Supabase. When building those flows, use a separate development project and review [`supabase-queries.md`](supabase-queries.md) alongside the tutorial. It is a collection of SQL notes, including a standalone function body and a later complete definition, rather than an ordered database migration to paste and run as a whole.

The completed app needs private `generated_images` and `training_data` buckets, ownership policies, database functions/triggers, and Supabase Auth URLs and email templates. Account creation or copying the notes alone does not provide a working backend. Follow the final repository's setup guide when it becomes available to you.

### 5. AI Model Links

Visit these links to set up your AI models:
- [Flux Dev LORA model trainer](https://replicate.com/ostris/flux-dev-lora-trainer/train)
- [Flux Dev Model](https://replicate.com/black-forest-labs/flux-dev)
- [Flux Schnell Model](https://replicate.com/black-forest-labs/flux-schnell)

For stock images (not for training), I have used [Lummi AI](https://www.lummi.ai/)

These are references for integrations you add during the tutorial. Check model availability, provider costs, and the applicable model and image licenses for your intended use before training, deployment, or redistribution.

### 6. Model Training Requirements

When training your custom model, ensure:
- 10-15 images in total
- Recommended breakdown for 12 images:
  - 6 face closeups
  - 3-4 half body closeups
  - 2-3 full body shots
- No accessories on face/head
- Different expressions, clothing, backgrounds
- 1:1 resolution (1048x1048 or higher)
- Images under 45MB total size

### 7. Stripe Setup

Watch our detailed video tutorial for Stripe integration setup: [Stripe Setup Tutorial](https://www.youtube.com/watch?v=7AQNeii5K7E&t=27960s)

Billing is implemented during the tutorial and remains a feature of the completed app. Use your own Stripe test-mode account and keys while building and validating it. This scaffold has no Checkout or webhook implementation.

### 8. Start Development Server

```bash
npm run dev
```

Visit `http://localhost:3000` to see the initial Next.js page. Start implementing the tutorial in `src/app/page.tsx`.

### 9. Check the Scaffold

```bash
npm run lint
npm run build
npm run start
```

The starter has no automated test script. A successful scaffold build does not validate the service integrations shown in the video. Review dependency audit results and test the completed authentication, storage, payments, training, and email flows before deployment.

## 📦 Project Structure

```
├── src/app/            # Initial Next.js page, layout, styles, and fonts
├── public/             # Tutorial assets and starter icons
├── screenshots/        # Completed tutorial reference screenshots
├── supabase-queries.md # Tutorial SQL notes
└── package-lock.json   # npm dependency lockfile
```

## 💰 Pricing Plans

These are examples from the completed tutorial. The starter has no billing or credit enforcement.

- **Hobby**: 1 trained model/month, 100 images/month
- **Pro**: 2 trained models/month, 300 images/month
- **Enterprise**: 5 trained models/month, unlimited images

## 📝 Source Access and License

The final-source destination is [Pictoria-AI-Final](https://github.com/codebucks27/Pictoria-AI-Final), with public access and license terms for the planned free release still pending. This starter currently has no checked-in license file; repository visibility alone does not establish a reuse license. The maintainer needs to clarify the applicable terms, including third-party assets.

## 🎥 Tutorial Video

For a complete setup walkthrough, check out our [video tutorial](https://youtu.be/7AQNeii5K7E).

## 🌟 Show Your Support

Give a ⭐️ if this project helped you!

If you have any question or want a custom build for your business, you can reach out to me via:

- E-mail : codebucks27@gmail.com
- Twitter: https://twitter.com/code_bucks
- Instagram: https://www.instagram.com/code.bucks/

MyChannel: https://www.youtube.com/codebucks
My Website: https://devdreaming.com/

## From the creator

SmartHeadshots is my separate hosted product for [professional AI headshots](https://www.smartheadshots.ai/professional-headshots).

Languages: [Deutsch](https://www.smartheadshots.ai/de/business-portrait) · [Español](https://www.smartheadshots.ai/es/foto-corporativa).
