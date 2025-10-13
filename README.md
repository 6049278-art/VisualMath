# Visualmath
Visualmath is an interactive Python-based whiteboard application built with Tkinter, designed for exploring mathematical concepts through visual, node-based computations. Users create colorful point units (yellow for inputs like variables, red for bases/scalars, blue for outputs/operations) to perform real-time addition, multiplication, logarithmic functions, and their inverses. Drag nodes to rearrange, link outputs for propagation, edit values via double-click or scroll, and use timers/deltas for dynamic updates—perfect for educators, students, or anyone visualizing math ideas on a dark-themed canvas.
## Features

Interactive Node Creation: Ctrl+Double-Click to spawn tri-color units (yellow/red inputs → blue output) with instant arrows and value labels.
Dynamic Operations: Right-click blue nodes to enable addition (+), multiplication (*), logarithmic (Log/Root/Base) and their inverses, or Integration via Riemann sums (∑ with history tracking and accumulation).
Value Editing & Linking: Double-click labels to edit, scroll for increments
Timers & Deltas: Right-click red/yellow nodes for "t" (1/sec auto-increment) or "delta" (custom step input) modes.
Manipulation Tools: Drag singles/groups (Shift+Click select), double-click arrows to reverse links (solve for "x"), Undo last unit, full Reset.
Visual Enhancements: Dark canvas (gray30 bg), white text/arrows for contrast, thousands separators in numbers, π/e legend, and Riemann history reports.
Extensible: Open-source for collaboration—add ops, export, or web ports via PRs!

## Installation
Since Visualmath is a standalone script (no PyPI package), clone the repo and run with Python 3.8+ (Tkinter included by default).
bashgit clone https://github.com/6049278-art/visualmath.git
cd visualmath
python whiteboard1.py  
For a portable executable (no Python needed): Use PyInstaller as described in CONTRIBUTING.md.
Requirements: None beyond Python stdlib (math, tkinter, collections).

## Usage
Launch the app:
python# Simply run the script
python whiteboard1.py
Quick Start Examples

#### Create a Basic Unit:

Ctrl+Double-Click on the canvas → Yellow/red points appear with blue output (all start at 1.0).
Drag blue to reposition; arrows follow.


#### Enable an Operation:

Right-click blue → "Addition" → "+" symbol appears; edit yellow to 5 (double-click label → type "5" → Enter) → blue updates to 6.0 (5 + 1 red).


#### Riemann Sum Demo:

Right-click blue → "Riemann Sum" → Scroll over yellow to accumulate values (e.g., +1 each time) → Left report shows history and total (sum * red width).


#### Linking Outputs:

Ctrl+Alt+Click two blue outputs → Dashed white arrow links them; changes propagate (with cycle prevention).



For advanced usage (e.g., timers on red/yellow: Right-click → "t" for auto +1/sec), see the in-app tooltips or demo video. Explore the code in whiteboard1.py—contributions welcome!
Contributing

## Contributing

Contributions are welcome! Please read the [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

This project is licensed under the [Apache License 2.0](LICENSE).

## Authors



> Star ⭐ the repo if you find it useful.  
> Open an issue or pull request for suggestions, improvements, or fixes!
