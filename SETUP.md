# Realtime chat setup

1. Copy `chat.html`, `admin-chat.html`, `chat.css`, `chat.js`, `admin-chat.js`, and `firebase-config.js` into your portfolio folder. `chat.css` must be beside `index.css`.
2. Replace placeholders in `firebase-config.js` with Firebase Web App config.
3. In Firebase Authentication, enable **Google** provider. Add your local testing domain and final portfolio domain to Authorized domains.
4. In Firebase Firestore Database, create a database, then paste `firestore.rules` under Firestore Database > Rules and publish.
5. Open `admin-chat.html`, sign in with your Google account, and copy the Firebase Authentication user UID from Firebase Console > Authentication > Users.
6. In Firestore, create a collection named `admins`. Create one document whose document ID is your copied UID. It may contain a field such as `email: "your-email@example.com"`.
7. Change the Hire Me button in `hire-me.html` to: `<a href="chat.html" class="btn"><i class="fa-solid fa-comments"></i> Discuss Your Project</a>`

Do not share `admin-chat.html` in your public navigation. You can open it directly to read and reply to visitor messages.