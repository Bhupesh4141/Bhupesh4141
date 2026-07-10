# DSA Streak Counter 🔥

A LeetCode-style problem submission tracker with streak counter, timer, and activity visualization built with vanilla JavaScript.

## Features

### 🔥 Streak Tracking
- **Current Streak**: Track consecutive days of problem-solving
- **Best Streak**: Keep track of your all-time high
- **Auto-Reset**: Streak automatically resets if you miss a day
- **Persistent**: All data stored in browser's localStorage

### ⏱️ Practice Timer
- Start, pause, and reset timer for practice sessions
- Tracks total practice time for the day
- Timer data persists across sessions
- Automatically saves when you log a problem

### 📊 Activity Visualization
- Weekly activity chart showing problems solved per day
- Visual representation of your consistency
- Color-coded activity levels

### 📈 Statistics Dashboard
- Easy, Medium, and Hard problem counters
- Total problems solved
- Detailed stats by difficulty level

### 📝 Problem Logging
- Quick problem entry with difficulty selection
- Recent problems list with timestamps
- Delete functionality for mistakes
- Auto-saves to localStorage

## Getting Started

### Installation

1. Clone or navigate to this directory
2. Open `index.html` in your web browser
3. Start logging problems and tracking your streak!

```bash
# No build process needed - just open the file!
open index.html
```

## Usage

### Logging a Problem

1. Enter the problem title in the input field
2. Select the difficulty (Easy, Medium, Hard)
3. Click "Log Problem" or press Enter
4. Your streak and statistics update automatically

### Using the Timer

1. Click **Start** to begin timing your practice session
2. Click **Pause** to temporarily stop the timer
3. Click **Reset** to clear the timer
4. Your practice time for today is automatically tracked

### Tracking Your Progress

- **Current Streak**: Updated when you log problems on consecutive days
- **Weekly Activity**: Visual chart showing your activity for the past 7 days
- **Statistics**: Real-time counts of easy, medium, and hard problems

## Data Storage

All data is stored locally in your browser using `localStorage`. This means:
- ✅ Your data persists between sessions
- ✅ No internet required after first load
- ✅ Completely private - no server involvement
- ⚠️ Data is lost if you clear browser cache

### Clearing Data

To reset all data and start fresh:
```javascript
// Open browser console (F12) and run:
localStorage.clear();
location.reload();
```

## File Structure

```
dsa-streak-counter/
├── index.html      # HTML structure
├── style.css       # Styling (dark theme)
├── script.js       # JavaScript functionality
└── README.md       # This file
```

## Features Explained

### Streak System
- Streak increases by 1 each day you log a problem
- Streak resets to 0 if you skip a day
- Best streak is recorded separately
- Automatic check at midnight

### Timer Feature
- Tracks hours:minutes format
- Accumulates throughout the day
- Combines multiple sessions
- Resets daily automatically

### Activity Chart
- Shows 7-day activity window
- Color intensity indicates problem count
- Hover for exact daily count
- Helps identify practice patterns

## Customization

### Change Theme Colors

Edit the CSS variables in `style.css`:

```css
:root {
    --primary-color: #0066ff;
    --danger-color: #ff4444;
    --success-color: #00cc66;
    --background: #0d1117;
    /* ... more colors ... */
}
```

### Modify Difficulty Tags

Edit the problem difficulty options in `index.html`:

```html
<select id="problemDifficulty">
    <option value="easy">Easy</option>
    <option value="medium">Medium</option>
    <option value="hard">Hard</option>
    <!-- Add more as needed -->
</select>
```

## Browser Compatibility

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Any modern browser with ES6 support

## Tips for Success

1. **Consistency is Key**: The streak system rewards consecutive days
2. **Log Immediately**: Log problems right after solving to maintain accurate streak
3. **Use the Timer**: Helps you track productive hours and identify your peak times
4. **Review Statistics**: Check your stats weekly to celebrate progress
5. **Set Goals**: Aim to beat your best streak!

## Troubleshooting

### Data Not Saving
- Check if localStorage is enabled in your browser
- Try a different browser if the issue persists
- Clear cache and reload

### Timer Not Working
- Ensure JavaScript is enabled
- Try refreshing the page
- Check browser console for errors (F12)

### Streak Not Updating
- Data updates when you log a problem
- Check that your system date/time is correct
- Problems must be logged on different days to increment streak

## Future Enhancements

Potential features to add:
- [ ] Export/backup data to JSON
- [ ] Difficulty statistics and graphs
- [ ] Problem categories/topics
- [ ] Cloud sync across devices
- [ ] Notifications/reminders
- [ ] Leaderboard system
- [ ] Problem source tracking (LeetCode, CodeForces, etc.)
- [ ] Time complexity tracking

## License

Free to use and modify for personal or educational purposes.

## Tips & Tricks

### Keyboard Shortcuts
- **Enter** in problem title field: Log problem
- **F12**: Open Developer Tools to access localStorage
- **Ctrl+Shift+Delete**: Clear browser data (Chrome)

### Best Practices
- Log problems immediately after solving
- Check your activity chart weekly
- Try to maintain a consistent daily streak
- Gradually increase difficulty as you improve

---

**Happy Coding!** 🚀 Keep that streak alive and build your problem-solving skills day by day.
