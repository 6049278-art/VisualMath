![Demo screenshot](Capture5.PNG)

## VisioMath
VisioMath is an interactive Python-based whiteboard application built with Tkinter, designed for exploring mathematical concepts through visual, node-based computations. Users create colorful point units (yellow for inputs like variables, red for bases/scalars, blue for outputs/operations) to perform real-time addition, multiplication, logarithmic functions, and their inverses. Drag nodes to rearrange, link outputs for propagation, edit values via double-click or scroll—perfect for educators, students, or anyone visualizing math ideas.
Free Version: Core operations (add/multiply/log) + text notes.
Premium ($9.99/mo): Unlock Time Timers & Riemann Sums—get your key via upgrade link!

## Features

Interactive Node Creation: Ctrl+Double-Click to spawn tri-color units (yellow/red inputs → blue output) with instant arrows and value labels.
Dynamic Operations (Free): Right-click blue nodes to enable addition (+), multiplication (*), logarithmic (Log/Root/Base) and their inverses.
Riemann Sum Demo (Premium): Right-click blue → "Riemann Sum" → Scroll over yellow to accumulate values (e.g., +1 each time) → Left report shows history and total (sum * red width).
Value Editing & Linking: Double-click labels to edit, scroll for increments (0.1 steps in free; custom in premium via deltas).
Timers & Deltas (Premium): Right-click red/yellow nodes for "t" (1/sec auto-increment) or "delta" (custom step input) modes.
Manipulation Tools: Drag singles/groups (Shift+Click select), double-click arrows to reverse links (solve for "x"), Undo last unit, full Reset.
Visual Enhancements: Dark canvas (gray50 bg), white text/arrows for contrast, thousands separators in numbers, π/e legend, and (premium) Riemann history reports.
Text Notes: Double-click canvas for editable multiline notes; drag via black handle dot.

Extensible: Open-source for collaboration—add ops, export, or web ports via PRs!

## Installation
**Free Version:**  
Clone the repository and run with Python 3.8+ (Tkinter included by default):

```bash
git clone https://github.com/6049278-art/VisualMath.git
cd VisualMath
python whiteboard1.py
```

No extra libraries required—just standard Python!

**Premium Version:**  
After you receive a premium key (via upgrade/donation), set your key before running:

```bash
# In your terminal, set the environment variable:
export PREMIUM_KEY='your_key'
python whiteboard1.py
```
- On Windows, use:
  ```
  set PREMIUM_KEY=your_key
  python whiteboard1.py
  ```

Unlock advanced features (Timers & Riemann Sums) after setting your key.

## Usage
Launch the app:


### Create a Basic Unit:

Ctrl+Double-Click on the canvas → Yellow/red points appear with blue output (all start at 1.0).
Drag blue to reposition; arrows follow.

### Enable an Operation (Free):

Right-click blue → "Addition" → "+" symbol appears; edit yellow to 5 (double-click label → type "5" → Enter) → blue updates to 6.0 (5 + 1 red).

### Linking Outputs:

Ctrl+Alt+Click two blue outputs → Dashed white arrow links them; changes propagate (with cycle prevention).

### Text Notes:

Double-click empty canvas → Type notes (Shift+Enter for lines) → Enter to save; drag black dot to move.

### For advanced usage 
(e.g., timers on red/yellow: Right-click → "t" for auto +1/sec), Upgrade to premium. See the in-app tooltips or demo video: https://www.youtube.com/watch?v=z8bdmnErXxM. Explore the code in whiteboard1.py—contributions welcome!
Premium Features

Time Timers: Auto-increment values every second on red/yellow points.
Riemann Sums: Accumulate integrals with history reports.
Custom Deltas: Fine-tune scroll steps.
Unlock by emailing for a key and setting os.environ['PREMIUM_KEY'] = 'your_key' before running.

### Contributing
Contributions are welcome! Please read the CONTRIBUTING.md for guidelines.
### License
This project is licensed under the Apache License 2.0.
### Authors
BlueYellowline

Star ⭐ the repo if you find it useful.
Open an issue or pull request for suggestions, improvements, or fixes!
