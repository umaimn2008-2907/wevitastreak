# WeVita

**Together, through every step of care.**

WeVita is a responsive React + Vite healthcare-continuity demo with medication tracking, appointment management, medical-record demo UI, care-gap reminders, a care circle preview, and a daily medication streak.

## Run on Windows

1. Install Node.js LTS from https://nodejs.org/ if it is not already installed.
2. Extract this ZIP.
3. Open the extracted `WeVita` folder in VS Code.
4. In VS Code, select **Terminal → New Terminal**.
5. Run these commands from the folder that contains `package.json`:

```powershell
npm install
npm run dev
```

6. Open the `Local` URL printed by Vite, usually `http://localhost:5173/`.

You can also double-click `start-wevita.bat` after Node.js is installed.

## Medication streak

The dashboard includes a medication-streak card. In demo mode, a day is added to the streak when all currently scheduled medication check-ins are confirmed. Streak history is saved in the current browser's local storage, so it remains on that browser after refresh. It is not yet synced across devices or accounts.

## Demo-mode notes

- This project uses synthetic demo information.
- Medication, appointment, and streak changes are stored in the current browser in demo mode.
- The records page demonstrates the interface; it does not upload actual files to cloud storage unless a secure backend is configured and implemented.
- Do not enter real patient data into this demo.

## Supabase configuration

Copy `.env.example` to `.env.local` and fill in the public project URL and anon/publishable key if configuring Supabase. Never put a Supabase service-role key in frontend environment variables. Review and test the SQL migration and Row Level Security policies before using real data.

## Build

```powershell
npm run build
npm run preview
```
