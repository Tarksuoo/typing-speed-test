Typing Speed Test
A terminal-based typing speed test written in Python. Measures your words per minute (WPM) and accuracy, saves your scores locally, and tracks your personal best across sessions.
Features

Randomized word prompts every round
WPM calculation using the standard 5-characters-per-word formula
Character-level accuracy measurement
Score history saved to a local JSON file
Personal best tracking
Diff view showing exactly where you made mistakes

How to run
Make sure you have Python 3.10 or higher installed. No external libraries required.
bashgit clone https://github.com/yourusername/typing-speed-test.git
cd typing-speed-test
python typing_speed_test.py
How it works
Each round generates a random sequence of common English words. Your input is timed from the moment you start typing until you press Enter. WPM is calculated as:
WPM = (characters typed / 5) / minutes elapsed
Accuracy is measured character by character, comparing your input against the original prompt. After each round, your score is appended to scores.json so your history persists between sessions.

Project structure
typing-speed-test/
├── typing_speed_test.py   # main program
├── scores.json            # auto-generated after first round
└── README.md

Example output
  Time      : 8.43 seconds
  WPM       : 64.1
  Accuracy  : 96.4%

  Breakdown:
  the quick brown fox jumps [o≠0]ver the lazy dog
