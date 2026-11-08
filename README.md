# Campus Connect

A responsive campus portal implementing the features shown in the reference image:

- Buy/sell books and gadgets (Marketplace)
- Lost & Found
- Club events
- Class notes
- Attendance tracker
- Personal timetable
- Placement updates
- Anonymous discussion forum

## Requirements
- Node.js 18+
- npm

## Run locally
```bash
npm install
cp .env.example .env
npm start
```
Open http://localhost:3000

## Getting started
1. Register using your name, college, email and a password of at least 8 characters.
2. Use **Create post** to publish marketplace, lost/found, event, notes, placement or forum posts.
3. Attendance and timetable data are private to the signed-in user.
4. Marketplace and lost/found posts can be marked resolved or deleted by their owner.

## Notes
- The app uses SQLite. Its database file (`campus-connect.db`) is created automatically on first start.
- This is a functional MVP starter, not a production-hardened deployment. Before public launch, add email verification, rate limiting, moderation/reporting, CSRF protections, backups, image uploads, privacy policy and stronger secret management.
- For a real college deployment, configure `JWT_SECRET` to a long random secret and use HTTPS.

## Student / Teacher login and timetable PDF
- Registration includes Student or Teacher account type.
- Timetable class entries include teacher name, subject, day, start/end time and room.
- Click Export timetable PDF on the timetable page, then choose Save as PDF in the browser print dialog.
