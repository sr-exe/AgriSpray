# AgriSpray AI

AgriSpray AI is a smart pesticide spraying system interface built for precision agriculture. It helps users capture live leaf images, analyze visible symptoms, and review scan analytics through a modern web dashboard.

The project focuses on reducing unnecessary pesticide usage by supporting targeted decisions instead of blanket spraying.

## Overview

This application provides:

- live camera-based leaf capture
- on-device visual symptom screening
- scan history with real-time analytics
- weekly reporting and disease distribution charts
- system flow and technology overview pages
- responsive UI with light and dark mode

## Key Features

- Live Detection: Opens the device camera, captures a leaf frame, validates image quality, and checks for visible symptoms.
- Smart Validation: Rejects scans when no clear leaf is detected or when the frame is too dark, blurry, or overexposed.
- Real-Time Analytics: Stores valid scans locally and updates dashboard numbers and charts from real scan history.
- Interactive UI: Includes animations, themed navigation, polished cards, and tab-based analytics views.
- Theme Support: Users can switch between light and dark mode.

## System Flow

The intended workflow is:

1. Capture a plant leaf image using the live camera.
2. Validate the image quality and confirm that a leaf is clearly visible.
3. Analyze visible color and stress cues from the captured frame.
4. Classify whether symptoms are present.
5. Trigger spray logic only for valid symptom-positive detections.
6. Save the scan result into analytics and dashboard history.

## Tech Stack

Frontend:

- React
- TypeScript
- Vite
- Tailwind CSS
- shadcn/ui
- Framer Motion
- Recharts
- React Router
- next-themes

Project / Tooling:

- ESLint
- Vitest
- Playwright

Conceptual / Extended Stack Referenced in UI:

- TensorFlow / Keras
- OpenCV
- Python + Flask
- Arduino integration for spray hardware

## Project Structure

```text
src/
  components/        Reusable UI and feature components
  components/ui/     UI primitives
  hooks/             Custom hooks
  lib/               Shared utilities and scan-history logic
  pages/             Route-level pages
public/              Static assets
```

## Local Development

### Requirements

- Node.js 18+ recommended
- npm

### Install

```bash
npm install
```

### Run the app

```bash
npm run dev
```

The Vite development server runs on the configured local host and port from the project setup.

### Build

```bash
npm run build
```

### Test

```bash
npm test
```

## Notes About Detection

The current detector uses front-end visual heuristics, not a trained medical-grade model. It improves user experience by:

- confirming that a leaf is actually present
- checking blur, glare, and darkness
- avoiding false result cards on invalid captures

For production-grade disease classification, the next step would be integrating a trained ML model through a backend API.

## Future Improvements

- backend model inference with TensorFlow / Flask
- real disease dataset integration
- hardware-linked spray controller workflow
- authentication and multi-user dashboards
- cloud storage for scan history and reports
- exportable scan logs and reports

## Contributors

- Shaikh Rizwan
- Shubham Rathod
