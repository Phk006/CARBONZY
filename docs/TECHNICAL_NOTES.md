# Technical Notes

## Architecture

CARBONZY is a static single-page application contained in `index.html`.

It uses:

- HTML for structure
- CSS for layout, animation, and responsive styling
- Vanilla JavaScript for state and interactions
- GitHub Pages for static hosting

## State Management

Runtime state is stored in a JavaScript object named `S`.

The current prototype tracks:

- Coins
- Lifetime coins
- Steps
- Completed habits
- Plastic disposal count
- Streak
- Green score
- Step coins
- Purchases
- Badges
- Challenge progress
- Camera state
- Audio state

State is not persisted to local storage or a backend.

## Navigation

The app uses multiple full-screen sections and toggles the active screen through JavaScript.

Main screens:

- `splash`
- `home`
- `challenges`
- `market`
- `profile`
- `camera`

## Camera

The recycling flow uses `navigator.mediaDevices.getUserMedia` when camera access is available.

If camera access fails, the app falls back to a generated demo capture on canvas.

## Audio

The app initializes a small Web Audio oscillator after the user starts the app. This avoids browser autoplay restrictions.

## Browser Compatibility

Recommended browsers:

- Chrome
- Edge
- Firefox
- Safari

Mobile browsers should work, though camera behavior can vary by device and permissions.

## Known Limitations

- No permanent user accounts
- No data persistence after refresh
- No backend validation for recycling
- Product redemption is simulated
- External font and video resources require network access

## Possible Next Technical Improvements

- Add local storage persistence
- Split HTML, CSS, and JavaScript into separate files
- Add a backend API
- Add authentication
- Add database-backed users, badges, and leaderboard
- Replace demo camera verification with a real review or ML verification flow

