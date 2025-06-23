# Pomodoro Timer Web App - Implementation Guide

A minimal, reliable Pomodoro timer with background audio notifications that work even when the browser tab is inactive.

## Features

- Simple, clean interface
- Configurable timer (1-999 minutes)
- Enhanced notification system:
  - Repeating audio alerts until acknowledged
  - Persistent system notifications
  - Prominent visual feedback
  - Customizable notification settings
- Reliable audio notifications even when the tab is in the background
- Visual feedback (enhanced flashing) when the timer completes
- System notifications with user interaction (if permitted by the browser)
- Fully keyboard accessible
- Screen reader friendly

## How to Use

1. Open `index.html` in Chrome browser
2. Enter a time in minutes (1-999)
3. Click "Start" to begin the timer
4. The timer will count down in MM:SS format
5. When the timer reaches 00:00:
   - Audio notifications will play (repeating until acknowledged)
   - The timer display will flash prominently
   - A persistent system notification will appear (if permitted)
   - The timer will reset to the original time

You can pause the timer at any time by clicking the "Pause" button. The "Reset" button will reset the timer to the originally configured time.

### Notification Settings

The Pomodoro Timer now includes customizable notification settings:

1. Open the "Notification Settings" section by clicking on it
2. Set the number of times notifications should repeat (1-10)
3. Click "Test Notifications" to test the notification system without waiting for a timer to complete
4. Click any notification or interact with the app to acknowledge and stop repeating notifications

![Notification Settings and Permission Handling](assets/img/notification%20handling.png)

## Implementation Details

This implementation meets all the requirements specified in the project brief:

### Core Timer Functionality

- Single HTML page with configurable timer input
- Timer display showing MM:SS format countdown
- Start/pause button controls
- Timer resets to original configured time when finished

### Background Audio Notifications

- Utilizes Web Audio API for reliable background playback
- Handles Chrome's autoplay policies and permission requirements
- Provides clear user feedback when permissions are needed

### Multiple Notification Methods

- Enhanced audio notifications:
  - Two-tone pleasant chime
  - Repeats until acknowledged
  - Uses multiple audio APIs for better background tab reliability
- Improved visual feedback:
  - Eye-catching color changes
  - Animation effects
  - Persistent until acknowledged
- Interactive system notifications:
  - Remains visible until clicked
  - Focuses window when clicked
  - Shows clear instructions

![System Notifications Example](assets/img/system_notifications.png)

### Accessibility Features

- Proper semantic HTML structure
- ARIA attributes for screen readers
- Keyboard navigation support
- Visual focus indicators
- Screen reader announcements for timer status

## Testing

A comprehensive test script is included in `tests.js`. To run the tests:

1. Open `index.html` in Chrome
2. Open Chrome DevTools (F12 or Ctrl+Shift+I)
3. Go to the Console tab
4. Type `PomodoroTests.runAllTests()` and press Enter

The test script will run automated tests and provide instructions for manual tests.

### Key Test Scenarios

- **Background Audio Test**: Set a short timer (30 seconds), switch to another tab, verify sound plays when timer ends
- **Permission Testing**: Test with Chrome's sound/notification permissions both allowed and blocked
- **Tab Inactive Test**: Verify timer continues counting down accurately when tab is not focused
- **Input Validation**: Test with various inputs (negative numbers, zero, very large numbers)

## Browser Compatibility

This application is designed primarily for recent versions of Chrome desktop browser. It uses the following web technologies:

- Web Audio API for reliable background audio
- Document Visibility API for background tab detection
- Notifications API for system notifications

## Limitations

- Audio may not work if browser policies block autoplay without user interaction
- System notifications require explicit user permission
- Some older browsers may not support all features

## Troubleshooting

- **No sound playing**: Check browser audio permissions and ensure volume is turned up
- **Timer not counting down accurately in background**: Browser throttling may affect timing in background tabs
- **System notifications not appearing**: Check notification permissions in browser settings
