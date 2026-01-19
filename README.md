# AI Study Planner & Productivity App

A smart study planning application that helps students and self-learners create intelligent study schedules based on deadlines, difficulty, and available time.

## Features

### 🎯 Task Prioritization with AI Suggestions
- Automatically calculates task priority based on:
  - Deadline urgency
  - Task difficulty (easy/medium/hard)
  - Estimated hours required
- Provides intelligent suggestions for task management
- Visual priority indicators

### 📅 Daily/Weekly Study Plans
- AI-generated study schedules
- Automatic time allocation based on priorities
- Customizable daily study hours
- View plans by day or week
- Smart session scheduling with breaks

### 📊 Progress Tracking & Statistics
- Real-time progress monitoring
- Completion rate tracking
- Task status management (pending/in-progress/completed)
- Visual progress bars
- Detailed statistics dashboard

### ⏱️ Focus Timer (Pomodoro)
- 25-minute work sessions
- 5-minute breaks
- 4-cycle Pomodoro technique
- Visual circular progress indicator
- Persistent timer state
- Start, pause, and reset controls

## Tech Stack

- **React 18** - UI framework
- **TypeScript** - Type safety
- **Vite** - Build tool and dev server
- **Tailwind CSS** - Styling
- **date-fns** - Date manipulation
- **lucide-react** - Icons
- **LocalStorage** - Data persistence

## Getting Started

### Prerequisites

- Node.js 18+ and npm

### Installation

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

3. Open your browser and navigate to `http://localhost:5173`

### Building for Production

```bash
npm run build
```

The built files will be in the `dist` directory.

## Usage

### Creating Tasks

1. Click "New Task" in the header
2. Fill in task details:
   - Title (required)
   - Description
   - Deadline (required)
   - Estimated hours (required)
   - Difficulty level
   - Tags (comma-separated)
3. Click "Create Task"

### Managing Tasks

- **Edit**: Click the edit icon on any task
- **Delete**: Click the delete icon (with confirmation)
- **Start**: Click "Start" to mark a task as in-progress
- **Complete**: Click "Mark Complete" when finished

### Study Plans

- Switch to "Study Plan" view
- Choose Daily or Weekly view
- Adjust daily study hours as needed
- View AI-generated study sessions

### Pomodoro Timer

- Navigate to "Focus Timer"
- Click "Start" to begin a work session
- Timer automatically switches between work and break periods
- Complete 4 cycles for a full Pomodoro session

### Progress Tracking

- View overall statistics in the "Progress" tab
- See completion rates, task counts, and time tracking
- Monitor your study progress over time

## AI Scheduling Algorithm

The app uses a smart priority calculation system:

1. **Urgency Factor** (50% weight): Based on days until deadline
2. **Difficulty Factor** (30% weight): Harder tasks get higher priority
3. **Time Factor** (20% weight): Tasks requiring more hours get prioritized when deadlines are close

Tasks are automatically sorted by priority, and study plans are generated to optimize your time allocation.

## Data Storage

All data is stored locally in your browser's localStorage:
- Tasks and their details
- Study sessions
- Pomodoro timer state

Your data persists between sessions and is never sent to external servers.

## License

MIT
