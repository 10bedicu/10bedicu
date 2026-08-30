<a href="https://10bedicu.org/">
<p align="center">
  <img src="https://images.ctfassets.net/kftzwdyauwt9/Uw8hmWd17OgUKHrKg02r6/1b8c9fdf236bd3f01f6945a8d382ed8f/10BedICU.png?w=1600&h=900&fit=fill"
       alt="10BedICU Banner"
       width="100%"
       style="border-radius: 15px;">
</p>
</a>

<p align="center">
  <b>10BedICU is an open-source initiative to rapidly deploy 10-bed ICU units in rural government hospitals as part of the Open Healthcare Network.</b>
</p>

<p align="center">
  <a href="https://10bedicu.org" target="_blank">🌐 Public Website</a> •
  <a href="https://github.com/ohcnetwork/10bedicu" target="_blank">🚀 GitHub Repository</a>
</p>

---

## Project Overview

**10BedICU** is a web portal that supports the deployment and management of 10-bed ICU units across rural areas in India. Initiated during the COVID-19 Delta wave, the project is a critical component of the Open Healthcare Network (formerly CoronaSafe Network). By integrating with the CARE backend (an open-source EMR system), 10BedICU provides real-time data on ICU capacity, hospital registrations, and tele-ICU services to help public and private stakeholders coordinate critical care services.

Learn more about the [Open Healthcare Network](https://ohc.network/) and the [CARE platform](https://care.ohc.network).

---

## Tech Stack

- **Next.js (React 17):** Server-side rendering and optimized routing for fast, scalable web applications.
- **Tailwind CSS:** Utility-first CSS framework for building modern, responsive UI designs.
- **Google Maps Integration:** Uses `google-map-react` to display interactive maps of ICU locations.
- **Backend Integration:** Connects to the CARE backend (Django/DRF) for dynamic data on hospitals, patients, and ICU status.
- **Deployment:** Hosted on Vercel for continuous deployment and fast global delivery.

---

## Installation & Setup

### Prerequisites

- [Node.js](https://nodejs.org/) v14+ and npm installed.

### Local Development

1. **Clone the Repository**

   ```bash
   git clone https://github.com/ohcnetwork/10bedicu.git
   cd 10bedicu
   ```
2. **Install Dependencies**

   ```bash
   npm install
   ```
3. **Start the Development Server**

   ```bash
   npm run dev
   ```

   Open [http://localhost:4000](http://localhost:4000) in your browser. The page will automatically reload on code changes.
4. **Environment Configuration**
   If you need to use external APIs (e.g., Google Maps), create a `.env.local` file in the root and add your environment variables

### Production Deployment

#### Using Vercel

- Connect the repository to [Vercel](https://vercel.com) for automatic builds and deployments.
- Set required environment variables in Vercel’s project settings.
- Push to the main branch to trigger a deployment.

#### Self-Hosting

1. **Build the Application**

   ```bash
   npm run build
   ```
2. **Start the Production Server**

   ```bash
   npm start
   ```

   The app will be served on port 4000. Ensure your environment variables are set for production.

---

## File Structure

- **`components/`**: Reusable React components (e.g., Header, Footer, UI widgets).
- **`pages/`**: Next.js pages defining routes (e.g., `index.js` for the homepage).
- **`data/`**: Static data files (JSON/CSV) used for content, configurations, or constants.
- **`map_data/`**: Geographical data (e.g., GeoJSON files, hospital coordinates).
- **`lib/`**: Utility functions and helpers (e.g., API calls, formatting).
- **`scraper/`**: Scripts used to gather or update hospital/ICU data.
- **`public/`**: Static assets like images, logos, and the favicon.
- **Configuration Files**: `next.config.js`, `tailwind.config.js`, `.gitignore`, and `package.json` configure the project.

---

## Maintainers & Community

- **Project Maintainers:**10BedICU is maintained by members of the [OHC Network](https://github.com/orgs/ohcnetwork/people). Their dedication ensures continuous improvement and support for the project.
- **Join Our Community:**
  Connect with us and other contributors via our [Slack community](https://slack.ohc.network/). Whether you have questions, ideas, or need support, we’d love to hear from you!

---

Happy coding and thank you for supporting 10BedICU – together, we can make critical care more accessible!
