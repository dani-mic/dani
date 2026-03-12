# Open Source Contributors Wall

> A **GDG on Campus HiLCoE** project for the *"Let's Dive into Open Source: Your Adventure in Teamwork"* event — March 14, 2026 | Addis Ababa, Ethiopia

A community-driven contributors wall where developers add their profile card by contributing a simple JSON file. Built to help beginners make their **first open-source contribution**.

## Features

- Profile cards rendered from JSON files
- Search and filter contributors by name or skill
- Animated card loading with staggered fade-in
- Live contributor counter with count-up animation
- Confetti celebration on page load
- Dark / Light mode toggle with saved preference
- Responsive design for all screen sizes
- Google-colored accent bar with GDG branding

## How to Contribute

1. **Fork** this repository
2. **Clone** your fork locally
3. **Create a branch** for your contribution
4. **Add your JSON file** in the `contributors/` folder
5. **Register your file** in `script.js`
6. **Open a Pull Request**

See the full step-by-step guide in [CONTRIBUTING.md](CONTRIBUTING.md).

## Contributor JSON Format

Create a file named `<your-github-username>.json` inside the `contributors/` folder:

```json
{
  "name": "Your Name",
  "github": "your-github-username",
  "avatar": "https://github.com/your-github-username.png",
  "bio": "A short bio about yourself",
  "skills": ["Skill 1", "Skill 2", "Skill 3"],
  "social": {
    "twitter": "",
    "linkedin": "",
    "website": ""
  }
}
```

Then open `script.js` and add your filename to the `contributorFiles` array:

```javascript
const contributorFiles = [
  "naol.json",
  "your-github-username.json"  // <-- add yours here
];
```

## Run Locally

Since the page uses `fetch()` to load JSON files, you need a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .
```

Then open `http://localhost:8000` in your browser.

## Project Structure

```
dev-toolkit/
├── contributors/          ← Add your JSON file here!
│   └── naol.json
├── assets/
│   ├── css/
│   │   └── style.css
│   └── images/
│       └── logo.png
├── index.html
├── script.js
├── README.md
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
└── LICENSE
```

## Event Details

| | |
|---|---|
| **Event** | Let's Dive into Open Source: Your Adventure in Teamwork |
| **Organized by** | GDG on Campus HiLCoE School of Computer Science & Technology |
| **Date** | Saturday, March 14, 2026 |
| **Time** | 9:00 AM – 10:30 AM (EAT) |
| **Location** | HiLCoE School, 4 Kilo, Addis Ababa, Ethiopia |
| **Event Page** | [GDG Community](https://gdg.community.dev/events/details/google-gdg-on-campus-hilcoe-school-of-computer-science-and-technology-addis-ababa-ethiopia-presents-lets-dive-into-open-source-your-adventure-in-teamwork/) |

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
