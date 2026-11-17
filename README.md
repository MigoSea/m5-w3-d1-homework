# Module 5 - Week 3 Day 1 Homework: React Facebook OAuth Login

## Project Overview
This repository contains the completed homework assignment for **Module 5 Week 3 Day 1 - Full Stack Web Development (WEB 403/603)** at Westcliff University.

The project demonstrates implementing Facebook OAuth 2.0 Login integration into a React.js application using `react-facebook-login` and `react-bootstrap`.

---

## Features Implemented
1. **Facebook OAuth 2.0 Integration:**
   - Configured `react-facebook-login` button with App ID `1088597931155576`.
   - Captures user profile fields: `name`, `email`, `picture` under `public_profile,user_friends` scopes.
   - Handles the OAuth access token response via `responseFacebook` callback.
2. **HTTPS Enforcement:**
   - Configured `"start": "HTTPS=true react-scripts start"` in `package.json` to comply with Facebook OAuth security requirements.
3. **Conditional State Rendering:**
   - **Unauthenticated State (`!login`):** Displays standard Login Form along with the Facebook OAuth login button.
   - **Authenticated State (`login`):** Displays the `<Home />` component showing the user's Facebook profile avatar, welcome message (`Welcome back {name}!`), and homepage confirmation text.
4. **Bootstrap 4 Styling:**
   - Responsive `<Card>` container with custom `.card-text form` styling in `App.css`.

---

## Directory Structure
```
m5-w3-d1-homework/
├── react-fb_login/
│   ├── public/
│   │   └── index.html
│   ├── src/
│   │   ├── App.css
│   │   ├── App.js
│   │   ├── index.css
│   │   └── index.js
│   └── package.json
├── .gitignore
└── README.md
```

---

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/MigoSea/m5-w3-d1-homework.git
   cd m5-w3-d1-homework/react-fb_login
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the application with HTTPS:
   ```bash
   npm start
   ```
4. Access the application at `https://localhost:3000`.
