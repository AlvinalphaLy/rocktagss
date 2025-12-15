# Meowvrick - Campus Cat Tracking Application

A full-stack web application to help the UTA community locate and interact with campus cats, promoting animal welfare awareness and community engagement.

**ACM Create Project | Fall 2025**

Directors / Contacts: Tobi and Prajit Viswanadha — DM on Discord

---

## 🐱 About The Project

Meowvrick is an interactive platform that features a campus map with real-time cat location tracking, user authentication, and an administrative dashboard for managing cat profiles and user permissions. The application helps students find friendly campus cats for stress relief while promoting responsible interaction with campus wildlife.

## Status & Links

- Phase: In Development (Not Yet Deployed)
- Communication: Discord #rocktags
- Open issues: use repo Issues; prefer labels `good first issue` and `help wanted` thoughtfully

---

## 🚀 Tech Stack

- **Frontend:** Next.js 15.5, React, TypeScript, TailwindCSS
- **Map Integration:** Leaflet.js for interactive campus mapping
- **Backend:** Next.js API Routes (serverless functions)
- **Database:** Cloud Firestore with real-time synchronization
- **Authentication:** Firebase Authentication with role-based access control
- **Deployment:** Ready for Netlify/Vercel deployment

## ✨ Key Features

- 🗺️ Interactive campus map with cat locations and building markers
- 🔐 User authentication with email verification
- 👨‍💼 Admin dashboard with CRUD operations for cat profiles and user management
- 🎯 Role-based access control (Admin/User permissions)
- 📱 Responsive design for mobile and desktop
- ⚡ Real-time database updates
- 🔄 Dynamic table columns that auto-adapt to Firestore schema

## Getting Started

### Prerequisites

- Node.js 20+
- npm or yarn
- Firebase account with project setup

### Environment Setup

1. Navigate to the project folder:

   ```bash
   cd rocktags
   ```

2. Copy the sample env file:

   ```bash
   cp .env.example .env.local
   ```

3. Add your Firebase credentials to `.env.local`:
   ```env
   FIREBASE_ADMIN_PROJECT_ID="your-project-id"
   FIREBASE_ADMIN_CLIENT_EMAIL="your-service-account-email"
   FIREBASE_ADMIN_PRIVATE_KEY="-----BEGIN PRIVATE KEY-----\n...\n-----END PRIVATE KEY-----\n"
   ```

### Installation

```bash
# Clone the repository
git clone https://github.com/AlvinalphaLy/rocktagss.git
cd rocktagss/rocktags

# Install dependencies
npm install

# Run development server
npm run dev
```

Visit `http://localhost:3000` to see the application.

---

## Repo Conventions

### Commits & Branches

- Use Conventional Commits. Examples:
  - `feat(ui): add dark mode toggle`
  - `fix(api): handle null user_id on login`
  - `docs(readme): clarify quickstart`
  - `chore(deps): bump eslint to v9`
- Branch names: `feat/<slug>`, `fix/<slug>`, `chore/<slug>`, `docs/<slug>`

### Pull Requests

- Prefer small, focused PRs
- Use the PR template: include testing steps, screenshots for UI changes, note breaking changes and rollback plan
- Request reviews from maintainers or CODEOWNERS

### Secrets & Configuration

- Never commit `.env` or credentials
- Use `.env` locally; keep `.env.example` updated so others know what is required
- For deployments, store secrets in platform settings (not in code)

---

## 📁 Project Structure

```
rocktags/
├── src/
│   ├── app/                    # Next.js app directory
│   │   ├── admin/             # Admin dashboard
│   │   ├── api/               # API routes (users, cats, banned)
│   │   ├── components/        # Reusable React components
│   │   ├── main/map/          # Interactive map page
│   │   └── login/             # Authentication pages
│   ├── config/                # Firebase configuration
│   ├── lib/                   # Utility functions
│   └── data/                  # Data fetching functions
├── public/                     # Static assets
├── .env.local                 # Environment variables (not committed)
└── package.json               # Dependencies
```

---

## 👥 Team & Contributors

**ACM Create Team Project**

- Directors / Contacts: Tobi and Prajit Viswanadha — DM on Discord

## 📄 License

This project is part of ACM Create at UTA.

## 🤝 Contributing

Contributions are welcome! Please follow the conventional commit format and submit PRs for review.

## 📧 Contact

For questions or support, reach out via Discord #rocktags channel.
