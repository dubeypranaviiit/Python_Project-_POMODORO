
# Pomodoro Timer Application

## Description
This **Pomodoro Timer** application is built using Python's `tkinter` library. The app follows the **Pomodoro Technique**, which alternates focused work sessions with short and long breaks to enhance productivity. It includes a visual interface with a timer overlaying a tomato image, color-coded phases (Work/Break), and checkmarks to track completed cycles.

---

## Features
- **Work and Break Timer**:
  - 25-minute work sessions.
  - 5-minute short breaks after every work session.
  - 20-minute long breaks after every 4 work sessions.

- **Dynamic UI Updates**:
  - Timer changes its text and color based on the current phase (Work or Break).
  - Displays checkmarks for completed work sessions.

- **Reset Option**:
  - Reset the timer, UI, and progress with a single button.

- **User-Friendly Interface**:
  - Easy-to-use buttons for starting and resetting the timer.
  - Clean and visually appealing layout.

---

## How It Works
1. **Start Timer**:
   - Click the **Start** button to initiate the first session.
   - The timer alternates between Work, Short Break, and Long Break phases based on the number of completed cycles (`REPS`).

2. **Countdown Mechanism**:
   - The timer counts down from the specified duration (Work: 25 mins, Short Break: 5 mins, Long Break: 20 mins).
   - When the timer reaches 0, it automatically moves to the next phase.

3. **Reset Timer**:
   - Click the **Reset** button to stop the timer and reset the app's state.

4. **Checkmarks**:
   - For each completed Work session, a checkmark (`✓`) is added.
   - After 4 work sessions, the checkmarks reset.

---

## Installation and Setup
1. **Prerequisites**:
   - Python 3.x installed on your system.
   - `tkinter` library (pre-installed with Python).

2. **Download the Code**:
   - Save the script as `pomodoro_timer.py`.

3. **Tomato Image**:
   - Ensure you have an image named `Tomato.png` in the same directory as the script.
   - The image will be used as a background for the timer.

4. **Run the Script**:
   - Navigate to the script's directory in your terminal or command prompt.
   - Run the script using:
     ```bash
     python pomodoro_timer.py
     ```

---

## Files
1. **`pomodoro_timer.py`**:
   - The main script containing the timer logic and UI code.

2. **`Tomato.png`**:
   - Image file used as the background for the timer.

---

## Code Structure
- **Constants**: Define colors, font, and timing durations.
- **Functions**:
  - `reset_timer`: Resets the timer, UI, and progress.
  - `start_timer`: Starts the timer for the appropriate session (Work/Break).
  - `count_down`: Handles the countdown mechanism and updates the UI.
- **UI Setup**:
  - Uses `Canvas` to display the timer over the tomato image.
  - Includes `Label` and `Button` widgets for user interaction.
- **Main Loop**: Keeps the application running and responsive.

---

## Screenshots
- **Work Session**:
  - A 25-minute countdown with a green header.
- **Short Break**:
  - A 5-minute countdown with a pink header.
- **Long Break**:
  - A 20-minute countdown with a red header.

---

## Future Enhancements
- **Customizable Timings**:
  - Allow users to set custom durations for work and break sessions.

- **Sound Notifications**:
  - Play a sound when switching between sessions.

- **Session Persistence**:
  - Save progress across sessions using a database or file.

---

## License
This project is free to use and modify.
