# Eyes-on-You
Official submission to HackHer413

An AI-powered Chrome extension that helps you stay focused by aligning your browsing with your intentions. Set your goal, browse (e.g. YouTube), and get gentle feedback when you're on track or when you're drifting.

![Chrome Extension](https://img.shields.io/badge/Chrome-Extension-4285F4?logo=googlechrome)
![Spring Boot](https://img.shields.io/badge/Backend-Spring%20Boot-6DB33F?logo=springboot)
![PostgreSQL](https://img.shields.io/badge/DB-PostgreSQL-336791?logo=postgresql)
![Gemini](https://img.shields.io/badge/AI-Google%20Gemini-4285F4?logo=google)

---

## What it does

1. **Set your intent**  Click the extension, start a session, and type your browsing goal (e.g. *"Learn how to cook pasta"*).
2. **Stay on track**  On YouTube, the extension captures what you're watching and uses **Google Gemini** to compare it with your intent. You get an **aligned** (green) or **distracted** (warning) popup.
3. **Focus mode**  The YouTube homepage and sidebar are blurred to reduce temptation.
4. **Notes & recap**  Add notes to videos; when you end the session, get an **AI-generated summary** and optional **quiz** (for educational content).

---

## Tech stack

| Layer        | Technology |
|-------------|------------|
| Extension   | Chrome Manifest V3, vanilla JavaScript |
| Backend     | Spring Boot (Java 21), Maven |
| Database   | PostgreSQL |
| AI         | Google Gemini API (multimodal: image + text) |

---

## Prerequisites

- **Chrome** (or Chromium-based browser)
- **Java 21** (JDK)
- **Maven** (or use the project’s `mvnw`)
- **PostgreSQL** (local or remote)
- **Google Gemini API key**

---

## Quick start

### 1. Database

Create a PostgreSQL database and user:

CREATE DATABASE productivity_extension;
-- Use your own username/password and set them in application.properties

