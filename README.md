# 🏋️‍♂️ PhysiqueTrack (RepVeda / GreenIron)
**Offline-First Vegetarian Muscle-Gain, Progressive Overload & Daily Discipline Tracker**

PhysiqueTrack is an Android and Web fitness companion designed for vegetarian lifters focused on lean mass gain. Every meal, workout set, step count, body measurement, and progress photo is stored 100% locally on-device with zero cloud dependency.

### ✨ Key Features
- **Double-Progression Overload Engine:** Automatically evaluates working sets against target rep ranges (e.g., `3 × 8–12`) and recommends equipment-specific load increments (`+1.0 kg`, `+2.0 kg`, `+2.5 kg`) only when all working sets hit the top of the range.
- **Indian Vegetarian Macro Calculator:** Explicitly separates **Raw/Dry** vs. **Cooked** food weights (e.g., 50g dry oats vs. 50g cooked oats) and includes 1-tap daily fixed staple checkboxes (Oats, Peanut Butter, Paneer, Moong Sprouts, Roasted Chana) right beside a live Water Intake station.
- **Word (`.docx`) Workout Plan Importer:** Upload any weekly gym split in `.docx` format to automatically parse Monday–Sunday exercises and log sets inline day-by-day.
- **Deduplicated Step & Activity Tracking:** Reconciles hardware `TYPE_STEP_COUNTER` readings across midnight rollovers and device reboots, deduplicates overlapping Health Connect windows, and supports manual walk fallback without GPS permissions.
- **7-Day Moving Average Body Analytics:** Smooths out daily scale fluctuations from hydration and glycogen to track true weekly lean mass gain alongside circumference logs and private on-device progress photos.

### 🛠 Tech Stack
- **Android Native:** Kotlin 2.0, Jetpack Compose (Material 3), SQLite (`SupportSQLiteOpenHelper`), Preferences DataStore, WorkManager, Health Connect API
- **Interactive Web / Hybrid Engine:** HTML5, Tailwind CSS, Chart.js, Mammoth.js & JSZip (for `.docx` parsing)
