# Architecture Overview – Jobbie iOS App

## Architectural Pattern
Jobbie follows a modular SwiftUI architecture inspired by the MVVM (Model-View-ViewModel)
pattern to ensure separation of concerns and scalability.

---

## Components

### Views
- Built using SwiftUI
- Responsible only for UI rendering
- Includes screens such as:
  - Home feed (job listings)
  - Job detail view
  - Search screen
  - Profile and authentication UI
- Uses SwiftUI navigation and layout components

---

### ViewModels
- Handle UI-related state and basic logic
- Act as a bridge between Views and Models
- Prepared for future backend and Firebase integration

---

### Models
- Represent job-related data such as:
  - Job title
  - Description
  - Location
- Currently uses hardcoded data for demonstration purposes

---

## Map Integration
- Uses Apple MapKit
- Displays job location on the job detail screen
- Designed to work with coordinate-based location data

---

## Data Flow
1. View triggers an action (e.g., selecting a job)
2. ViewModel processes the state or data
3. View updates automatically based on state changes

SwiftUI’s declarative UI model ensures automatic UI updates.

---

## Current Limitations
- Frontend-only implementation
- Hardcoded job data
- No backend or authentication integration yet

---

## Future Enhancements
- Firebase authentication
- Dynamic job data from backend
- Job posting and application workflow
- Deployment via TestFlight or App Store
