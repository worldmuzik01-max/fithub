# ⚡ ALEXFITNESSHUB

Welcome to **ALEXFITNESSHUB**, a world-class, AI-powered premium fitness platform engineered for high-performance athletes. It combines military calisthenics, gym bodybuilding schemes, tailored calorie-centric diets, high-precision progress tracking, and interactive diagnostic systems into a single responsive digital space.

---

## 🌟 Key Capabilities

*   **🤖 AI Coach & Smart Plans**: Live custom workout schemes and culinary matrices generated dynamically based on your physical metrics, target weight, and chosen goals.
*   **⚔️ Specialized Athletics**:
    *   **Calisthenics Engine**: Progressive bodyweight routines from beginner moves to elite planetary levers.
    *   **Home Workouts**: Minimalist training templates optimized for high-intensity interval conditioning.
    *   **Gym Dominance**: Heavy mechanical loading schemes built for hypertrophy and strength limits.
*   **🥗 Chef's Elite Nutrition Matrix**: Personalized daily macro/calorie trackers alongside delicious recipes (including premium regional power proteins like grilled Croaker fish, Jollof rice bowls, and baked Moi Moi).
*   **🛡️ Automated Diagnostic Console**: A secure production-ready console displaying Firebase initialization status, active OAuth authorization channels, active hostname validations, and testing triggers.
*   **💳 Financial Checkout Engine**: Integrated with Monnify Config layouts for secure subscription tiers and premium access control.
*   **🔐 Best-in-Class Security & Identity**: Powered by Firebase Auth with password resets, secure email verification, and a dual-strategy (Popup + Redirect fallback) Google Sign-In system.

---

## 🛠️ Technology Stack & Architecture

This application is built as a highly optimized, fully responsive **Full-Stack SPA** running inside React 18, Vite, and an Express proxy server:

*   **Frontend**: React (TypeScript), Tailwind CSS for streamlined responsive utility styling, and `lucide-react` for aesthetic displays.
*   **Backend Server**: Node.js & Express (`server.ts`) implementing robust API routes, database syncer paths, and a fallback handler for static server deployments.
*   **Database**: Google Cloud Firestore for dynamic user metadata, subscription tracking, and exercise logs.
*   **Authentication**: Firebase SDK with active persistence trackers.

---

## ⚙️ Environment Configuration

To configure local development or production environments on cloud instances (such as Cloud Run or Render), create a `.env` file at the root of the project with the following structures:

```env
# SERVER-SIDE PORT (Exposed automatically to Node processes)
PORT=3000

# VITE-SPECIFIC FIREBASE CLIENT VARIABLES
VITE_FIREBASE_API_KEY=AIzaSyBCEDeHlRU4HmzgqWlFy-7r6Nf23wxSi3o
VITE_FIREBASE_PROJECT_ID=alex-6ee81
VITE_FIREBASE_AUTH_DOMAIN=alex-6ee81.firebaseapp.com
VITE_FIREBASE_STORAGE_BUCKET=alex-6ee81.firebasestorage.app
VITE_FIREBASE_MESSAGING_SENDER_ID=934491984930
VITE_FIREBASE_APP_ID=1:934491984930:web:d641806f0f70e527afa67b
VITE_FIREBASE_MEASUREMENT_ID=G-V73ZQ93K40

# SECURE BACKEND INTEGRATIONS (Server.ts)
GEMINI_API_KEY=your_gemini_api_key_here
MONNIFY_API_KEY=your_monnify_api_key_here
MONNIFY_SECRET_KEY=your_monnify_secret_key_here
```

---

## 🚀 Local Development Workflow

Start building or custom-styling with the built-in development servers:

### 1. Install Base Dependencies
```bash
npm install
```

### 2. Launch Development Servers
This boots the server.ts TSX runtime on port `3000`:
```bash
npm run dev
```

### 3. Production Compilation & Packaging
Bundles the frontend client via Vite and bundles the backend server into a single standalone CommonJS application in `dist/server.cjs` via `esbuild`:
```bash
npm run build
```

### 4. Run Production Executable
```bash
npm start
```

---

## 🛡️ Production Domain & OAuth Setup Guidance

When hosting on platforms like **Render** or **custom domains**, you must complete this standard Firebase security handshake to authorization:

1.  **Read Active Hostname**: Visit your application and copy its live address (e.g., `https://your-app.onrender.com`).
2.  **Add to Authorized Domains**:
    *   Open the [Google Firebase Console](https://console.firebase.google.com/).
    *   Navigate to **Authentication** (sidebar) > **Settings** (tab) > **Authorized Domains**.
    *   Click **Add Domain** and paste your deployed application URL.
3.  **Use Diagnostic page**: Navigate to `/auth/diagnostic` inside ALEXFITNESSHUB to confirm active domain sync. If blocked inside frames or browser restrictions, utilize the **Google Redirect Sign-In Fallback** option provided on the Login screen instead of Popups.

---

## 📁 Core Directory Map

```text
├── src/
│   ├── components/       # Premium Navigation, Footer, and layout systems
│   ├── context/          # AuthContext with dynamic session managers 
│   ├── lib/              # Firebase API setup and custom multi-lingual errors
│   ├── pages/            # Core athlete pages (Diets, Calisthenics, Coaching)
│   │   ├── Diagnostic.tsx # Automated live health diagnosis screen
│   │   └── ...           # Login, Sign-up, Onboarding screens
│   ├── types.ts          # Central TypeScript interfaces
│   └── main.tsx          # Initial core rendering mount
├── server.ts             # Express.js full-stack proxy & API handlers
├── firebase-applet-config.json # Base fallback credentials file
└── package.json          # Production packages & bundling script definitions
```

---
*Created and maintained with extreme athletic pride. Let's build your physical legacy!*
