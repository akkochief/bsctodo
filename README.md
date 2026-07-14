```markdown
# BscTodo — Advanced Task Management

A fully-featured task management application with integrated Pomodoro timer, built entirely with vanilla JavaScript. No frameworks, no dependencies — just open and use.

## Quick Start

1. Extract the zip file to any folder
2. Double-click `index.html` to open in your browser
3. Start managing your tasks instantly

All data is stored locally in your browser's `localStorage`. Your tasks, categories, and pomodoro sessions persist even after closing the browser.

## Features

### Task Management
- Create, complete, delete, and archive tasks
- Set priority levels: Low, Medium, High
- Assign due dates and time estimates
- Add subtasks, tags, and notes
- Drag and drop support (touch-friendly)
- Double-click any task to edit in detail

### Categories
- Create custom categories with 8 color options
- Filter tasks by category
- Delete categories with automatic task reassignment
- Color-coded visual organization

### Smart Filters & Search
- Filter by: All, Active, Completed, Archived
- Quick filters: Today, This Week, Overdue
- Real-time search across task text, tags, and notes

### Advanced Pomodoro Timer
- Focus, Short Break, Long Break modes
- Customizable durations (Focus: 1-120min, Short: 1-30min, Long: 1-60min)
- Visual circular progress dial with tick marks
- Session counter with dot indicators
- Auto-start after break (optional)
- Sound notifications on completion
- Keyboard shortcut: Space to start/pause

### Analytics & Insights
- **Productivity Score**: Dynamic scoring based on completed tasks, streaks, and pomodoro sessions
- **Level System**: Earn XP and level up
- **Weekly Chart**: Last 7 days task completion (animated bar chart)
- **Category Distribution**: Donut chart visualization
- **Priority Distribution**: Visual bar chart
- **Statistics**: Today's completions, streak counter, active tasks, completion rate
- **Streak Tracking**: Consecutive days with completed tasks

### Data Management
- Export data as JSON backup
- Import data from JSON backup
- Auto-backup every save
- Undo/Redo (Ctrl+Z / Ctrl+Y)
- Keyboard shortcuts for power users

### User Experience
- Dark/Light theme toggle
- Particle effects on task completion
- Responsive design (mobile, tablet, desktop)
- Keyboard accessible (focus outlines, shortcuts)
- Reduced motion support (prefers-reduced-motion)
- Smooth animations and transitions

### Keyboard Shortcuts
| Shortcut | Action |
|----------|--------|
| `Ctrl+N` | Focus task input |
| `Ctrl+F` | Focus search |
| `Ctrl+Z` | Undo |
| `Ctrl+Y` | Redo |
| `Space` | Start/Pause timer |
| `Escape` | Close modals |

## File Structure

```
bsctodo-main/
├── index.html   → Complete application (HTML + CSS + JS)
└── README.md    → Documentation
```

## Browser Support

Works on all modern browsers:
- Chrome 90+
- Firefox 88+
- Edge 90+
- Safari 14+
- Opera 76+

## Reset Data

To reset all data, open browser console (F12) and run:
```js
localStorage.removeItem("bsctodo_state_v6")
```

Or use the **Settings** panel → Reset button.

## Technical Details

- **Framework**: Vanilla JavaScript (no dependencies)
- **Storage**: localStorage with JSON serialization
- **Audio**: Web Audio API for chime sounds
- **Fonts**: Google Fonts (Outfit, JetBrains Mono) with fallback
- **Icons**: Font Awesome 6.5.1
- **Animations**: CSS transitions, keyframes, and requestAnimationFrame
- **Responsive**: CSS Grid, Flexbox, mobile-first approach

## Version History

### v6.0 (Current)
- Full redesign with premium gradient theme
- Level and XP system
- Productivity score
- Subtasks support
- Tags system
- Notes field
- Time estimates
- Advanced timer controls with custom durations
- Export/Import backup
- Undo/Redo
- Keyboard shortcuts
- Dark/Light theme
- Overdue task highlighting
- Archive functionality
- Quick filters (Today, Week, Overdue)
- Responsive mobile layout
- Particle effects
- Notification system

### v5.0
- Initial release with core features
- Task management with categories
- Pomodoro timer
- Basic statistics

## Customization

You can modify the following in the code:

- **Colors**: Edit CSS variables in `:root`
- **Timer defaults**: Change values in `DEFAULT_STATE.timer`
- **Category colors**: Modify `PALETTE` array
- **XP thresholds**: Adjust `xpThreshold` variable
- **Daily goals**: Modify `dailyGoals` object

## License

MIT License — Free for personal and commercial use.


