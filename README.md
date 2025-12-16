
#  Crypt Vault

**Crypt Vault** is a modern, text-based dungeon crawler written in Python.
It serves both as a playable game and a technical showcase demonstrating object-oriented design, state management, branching logic, persistence, and testing in a single, well-structured project.

---

##  Features

* **Turn-based combat** with critical hits, equipment bonuses, and flee mechanics
* **Exploration system** with rooms, traps, locked areas, and random events
* **Progression & leveling** with scaling stats and difficulty modes
* **Inventory & equipment system** (weapons, armor, consumables, keys)
* **Save & load system** using JSON serialization
* **Session statistics** (kills, damage, rooms explored, turns, etc.)
* **Polished CLI interface** using the `rich` library
* **Built-in test suite** for core game systems

---

##  What This Project Demonstrates

This project was designed as a **portfolio-grade Python application**, highlighting:

* Object-Oriented Programming (OOP)
* Centralized state management
* Logic branching and decision handling
* Error handling with custom exceptions
* Data serialization and persistence
* Clean CLI UX design
* Lightweight automated testing

---

##  Requirements

* Python **3.10+**
* `rich` library

Install dependencies:

```bash
pip install rich
```

---

##  How to Run

Start a new game:

```bash
python crypt_vault.py
```

Start with a specific difficulty:

```bash
python crypt_vault.py easy
python crypt_vault.py normal
python crypt_vault.py hard
```

Load a saved game:

```bash
python crypt_vault.py load savegame.json
```

Run the test suite:

```bash
python crypt_vault.py test
```

---

##  Saving & Loading

You can save or load at any time during gameplay:

```
save
load savegame.json
```

The entire game state (player, rooms, enemies, inventory, stats, turn count) is preserved.

---

##  Project Structure

```
crypt-vault/
│
├── crypt_vault.py        # Main game engine (single-file project)
├── crypt_vault.log       # Runtime debug logs
└── README.md             # Project documentation
```

*(Single-file by design to showcase architecture clarity without framework overhead.)*

---

##  Testing

The project includes a built-in test runner covering:

* Item system
* Combat logic
* Inventory management
* Navigation and error handling
* Save/load persistence
* Level progression


