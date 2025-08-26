# ManMode - Personal Dashboard

A personal dashboard application built with React, TypeScript, and Tailwind CSS.

## 🛠️ Tech Stack

- **Frontend**: React 18, TypeScript, Vite
- **Styling**: Tailwind CSS, Radix UI Components
- **State Management**: React Context API
- **Routing**: React Router v6

## 📁 Project Structure

```
src/
├── components/           # UI components
│   ├── ui/              # Radix UI based components
│   ├── AccountSettings.tsx
│   ├── AuthForm.tsx
│   ├── FitnessZone.tsx
│   ├── GoalsManager.tsx
│   ├── HabitTracker.tsx
│   ├── KnowledgeZone.tsx
│   ├── Navigation.tsx
│   ├── PomodoroTimer.tsx
│   ├── ProductivityZone.tsx
│   ├── UserProfile.tsx
│   ├── WorkoutSchedule.tsx
│   └── XPDisplay.tsx
├── contexts/            # React context providers
│   └── AuthContext.tsx
├── hooks/               # Custom hooks
│   ├── use-mobile.tsx
│   └── use-toast.ts
├── lib/                 # Utility functions
│   └── utils.ts
└── pages/               # Page components
    ├── Index.tsx
    └── NotFound.tsx
```

## 👥 Team Responsibilities (25% Each)

### 1. Nandhish
- `src/contexts/AuthContext.tsx`
- `src/components/AuthForm.tsx`
- Authentication flow
- User session management

### 2. Shreeraj
- `src/pages/Index.tsx`
- `src/pages/NotFound.tsx`
- Routing setup
- Page layouts

### 3. Abhinash
- `src/components/FitnessZone.tsx`
- `src/components/WorkoutSchedule.tsx`
- Fitness tracking features
- Data visualization

### 4. Sonohar
- `src/components/ProductivityZone.tsx`
- `src/components/PomodoroTimer.tsx`
- `src/components/HabitTracker.tsx`
- Productivity features

## 🚀 Getting Started

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```
4. Open [http://localhost:5173](http://localhost:5173) in your browser

## 📝 License

MIT
