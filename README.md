<div align="center">

# 🧬 VITalWatch (Prototype)

**Smart India Hackathon (Round 2) — Problem Statement 46**<br>
_A Next-Generation Clinical Trial Management System (CTMS) & Pharmacovigilance Platform_

[![Next.js](https://img.shields.io/badge/Next.js-15-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19-blue?style=for-the-badge&logo=react)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-4-38B2AC?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com/)
[![Clerk](https://img.shields.io/badge/Auth-Clerk-6C47FF?style=for-the-badge&logo=clerk)](https://clerk.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

</div>

---

## 📖 About the Project

**VITalWatch** is a production-quality frontend prototype designed to solve **Problem Statement 46** for the Smart India Hackathon. It serves as a unified Clinical Trial Management System (CTMS) and Pharmacovigilance (PV) module, envisioned for institutions like the All India Institute of Ayurveda (AIIA) and the National Pharmacovigilance Coordination Centre (NPvCC).

> **Note:** This is a prototype system running with **synthetic data only**. No real patient data is used or stored at any stage of this application.

Our goal is to bring the polished, real-time aesthetic of modern SaaS platforms (like Vercel or Linear) to regulated healthcare workflows, making data-dense clinical interfaces trustworthy, legible, and highly responsive.

## ✨ Key Features

- **Role-Based Workflows (RBAC):** Custom views and capabilities for Principal Investigators, Study Coordinators, Clinical Monitors, Ethics Committees, PV Officers, Admins, and Regulators.
- **Real-Time Pharmacovigilance (PV):** Live SAE (Serious Adverse Event) intake with semantic MedDRA coding suggestions and ticking regulatory countdown clocks (24h/14d deadlines).
- **Portfolio & Study KPIs:** Live count-up tiles and active Recharts curves comparing actual vs. expected trial enrolment.
- **Immutable Audit Trail:** Chronological, hash-chained audit logs with visual diff viewers and real-time chain verification for regulatory compliance.
- **Stub Mode Architecture:** The entire frontend can run fully detached from the backend using a local fixture-based API layer, ensuring seamless offline demonstrations.

## 🛠️ Tech Stack

This project is built using bleeding-edge web technologies to ensure maximum performance and developer experience:

- **Framework:** Next.js 15 (App Router) & React 19
- **Styling:** Tailwind CSS v4 & generic UI primitives (shadcn-inspired)
- **Animation:** Framer Motion (page transitions, count-ups, timeline tickers)
- **Authentication:** Clerk (`@clerk/nextjs`) with custom role-based routing
- **Data Visualization:** Recharts
- **Data Fetching:** TanStack Router & React Query

## 🚀 How to Run Locally

### Prerequisites

Make sure you have [Node.js](https://nodejs.org/) (v20+) or [Bun](https://bun.sh/) installed.

### Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

### Running Locally

To run the application for demonstration purposes locally, use **Stub Mode**. This bypasses the need for a live backend and uses our comprehensive synthetic data fixtures.

```bash
VITE_STUB_MODE=true npm run dev
```

Open [http://localhost:3000](http://localhost:3000) (or the port specified in your terminal) to view it in the browser.

## 🌐 Deploying to GitHub Pages

We have pre-configured a **GitHub Actions workflow** to automatically build and deploy this prototype to GitHub Pages in **Stub Mode**. 

Follow these steps to launch it successfully:

1. **Push your code to GitHub:**
   Ensure this repository is pushed to your own GitHub account.

2. **Enable GitHub Pages settings:**
   - Go to your repository on GitHub.
   - Click on **Settings** > **Pages** (on the left sidebar).
   - Under **Build and deployment** > **Source**, select **GitHub Actions**.

3. **Trigger the workflow:**
   - Go to the **Actions** tab in your repository.
   - You should see a workflow named `Deploy to GitHub Pages`.
   - The workflow will automatically run on every push to the `main` branch. 
   - *(Optional)* You can also click on the workflow and click **Run workflow** to trigger it manually.

4. **Access your live site:**
   Once the action completes (it usually takes 1-2 minutes), your site will be live! You can find the URL in the Settings > Pages menu or in the deployment summary in the Actions tab.

> **Routing Note:** Because this is a Single Page Application (SPA), the workflow automatically copies `index.html` to `404.html` during the build process to ensure that deep linking (like navigating directly to `/portfolio`) works perfectly on GitHub Pages.

## 👥 Meet the Team

This prototype was proudly designed and developed by:

- **Caleb Elisha Joseph**
- **Sreeja Kotra Reddy**
- **Kavin K**
- **Roxy**
- **Ishan**
- **Rakshitha S**

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<div align="center">
  <i>Built with ❤️ for the Smart India Hackathon</i>
</div>
