# 🕒 Digital Clock with Theme Switcher (Python Tkinter Project)

**📌 Project Overview**

This is a simple yet functional digital clock application built using Python’s Tkinter GUI toolkit.
It displays the current time in 12-hour format (with AM/PM) and allows users to switch between light and dark themes dynamically using a menu bar.

The clock updates every second, ensuring accurate real-time display.

## 🚀 Features

- ✅ Displays time in HH:MM:SS AM/PM format
- ✅ Live update every second (using Tkinter’s after method)
- ✅ Light and Dark theme options accessible via menu
- ✅ Clean, minimalistic UI
- ✅ Resizable window

## 💡 How it Works

- The app creates a main window using Tkinter.

- A menu bar allows users to choose between:

- Light theme → white background with black text

- Dark theme → dark blue background with black text

- When a theme is selected, a new frame is created and placed on the window, with a clock label inside it.

- A nested time() function fetches the current time using strftime() and updates the clock label every second using after(1000, time).

- The app starts with a default theme (light blue frame with clock).

## 🖥️ Code Highlights
```
def light_theme():
    # Creates a white frame with a black clock
    # Updates time every second using after()
```
```
def dark_theme():
    # Creates a dark blue frame with black clock text
```
```
def time():
    # Fetches time as string and updates label
    # Calls itself after 1000 ms (1 second)
```
```
theme_menu.add_command(label="Light", command=light_theme)
theme_menu.add_command(label="Dark", command=dark_theme)
```
👉 The theme switching is done via a menu bar dropdown, not buttons.

## ⚡ Technologies Used

- Python 3

- Tkinter (built-in GUI library)

- time module (strftime for time formatting)

## 💻 How to Run
1. Clone the repository
```
git clone https://github.com/Mazid2003/Digital-Clock-using-python-Tkinter.git

cd Digital-Clock-using-python-Tkinter

```

1️⃣ Make sure you have Python 3 installed.

2️⃣ Run the script:
```
python digital_clock.py
```

✅ The app window will open, showing the clock and theme menu.

## ✨ Possible Enhancements

- If you plan to showcase future ideas on GitHub, you can list:

- Destroy previous theme frames (so they don’t overlap on repeated switches)

- Add more themes (neon, green terminal, etc.)

- Add date display

- Show timezone

- Full-screen clock mode

## 📝 Summary for GitHub

- This is a beginner-friendly Python GUI project showcasing:

- Tkinter layout management

- Real-time clock updates

- Dynamic theme switching

It can serve as a base for more advanced clock apps!


