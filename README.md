# Kurippu

Kurippu is an elder-friendly, bilingual (English and Malayalam) medication management and prescription scanning application. Built with React and Vite, it leverages Gemini 1.5 Flash for accurate OCR to analyze prescriptions and keep users safe.

## Features

- **Gemini OCR Integration:** Accurately scans and analyzes prescriptions using Gemini 1.5 Flash multimodal OCR.
- **Bilingual Interface:** Seamlessly switches between English and Malayalam (EN/ML) across the entire application.
- **Elder-Friendly Design:** Designed with high contrast, large typography (22px+ fonts), and distinct Trust Blue / Safety Red accents for maximum readability and ease of use.
- **Safety and Conflict Alerts:** Implements a safety buffer by cross-checking current medications and allergies (e.g., Warfarin, Penicillin), presenting a full-screen red alert with an emergency call button if conflicts are detected.
- **Daily Med-Log:** A comprehensive daily dose checklist to track medication intake (TAKEN/കഴിച്ചു) with timestamps.
- **Smart Reminders:** Utilizes the Web Audio API for chime reminders and interval checks for dose schedules.
- **Persistent Storage:** Completely local and privacy-respecting, leveraging `localStorage` to save all scan history and dosage logs.
- **Persistent SOS Button:** One-tap emergency call footer always available across screens.

## Architecture & Tech Stack

- **Framework:** React + Vite
- **Styling:** Tailwind CSS (v4)
- **AI/OCR:** Google Gemini 1.5 Flash API
- **State Management:** React Hooks and local storage persistence

## Getting Started

Follow these steps to set up the project locally.

### 1. Prerequisites

Ensure you have Node.js and npm installed on your machine.

### 2. Setup API Key

You will need a Google Gemini API Key. Get a free key at: [Google AI Studio](https://aistudio.google.com/apikey).

Create a `.env` file in the root of the project and add your key:

```env
VITE_GEMINI_API_KEY=your_gemini_api_key_here
```

### 3. Installation

Install the project dependencies:

```bash
npm install
```

### 4. Running the Development Server

Start the application locally:

```bash
npm run dev
```

Open `http://localhost:5173` in your browser to view Kurippu.

## Build for Production

To create an optimized production build:

```bash
npm run build
```

## Contributing

Contributions are welcome! Please create an issue or submit a pull request if you want to help improve Kurippu.
