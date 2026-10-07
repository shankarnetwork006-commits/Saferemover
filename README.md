# SafeRemove AI V1

Mobile-first safety/report workflow prototype.

## Important
This app does not and cannot forcibly delete content from third-party platforms. It prepares/tracks legitimate, authorized reporting workflows. Final removal is controlled by each platform.

## Run
1. Install Node.js 20+.
2. `npm install`
3. Copy `.env.example` to `.env` and add Firebase web configuration.
4. `npm run dev`

## Firebase
Configure Authentication and Firestore, then deploy rules/functions with the Firebase CLI.

## AI
The included UI deliberately does not fake AI results. Connect Gemini or another approved moderation service on the server, with strict privacy/retention controls. Never expose `GEMINI_API_KEY` in browser code.

## Production checklist
- Authentication
- App Check
- Server-side AI moderation
- Rate limiting/abuse prevention
- Data minimization and retention deletion
- Official platform APIs/reporting workflows only
- Human review for high-impact cases
- Special child-safety escalation process
- Audit logging without storing sensitive media
