# 🔍 Digital Lost and Found System

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Anshul-lite/digital-lost-and-found-system/blob/main/digital_lost_and_found_system.ipynb)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter%20%2F%20Colab-orange.svg)
![Status](https://img.shields.io/badge/Status-Active-brightgreen.svg)
![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)

An interactive, lightweight **Digital Lost and Found Management System** developed in Python and Jupyter Notebook / Google Colab. It provides a tabbed graphical user interface powered by `ipywidgets` and handles data persistence using a local CSV storage engine.

---

## 🚀 Key Features

- **📝 Report Lost or Found Items**:
  - Structured input form to register item name, category, location, detailed description, and contact info.
  - Automatic unique ID assignment and timestamping.
- **🔎 Dynamic Search & Filtering**:
  - Full-text search across item names, locations, and descriptions.
  - Multi-criteria filters by item type (`All`, `Lost`, `Found`) and status (`Open`, `Claimed/Resolved`).
  - Real-time tabular output rendered using `pandas` and IPython display utilities.
- **🏷️ Claim & Resolution Tracking**:
  - Quickly mark items as resolved or claimed by Item ID.
  - Immediate database status synchronization.
- **💾 Automatic Data Persistence**:
  - Backed by `lost_and_found_db.csv` which initializes automatically on the first run.
- **🎨 Interactive Tabbed GUI**:
  - Intuitive interface structured with `ipywidgets.Tab`, `VBox`, and `HBox` components for a clean user experience in notebooks.

---

## 📊 Database Schema

The system persists items into `lost_and_found_db.csv` with the following schema:

| Column | Type | Description |
| :--- | :--- | :--- |
| `ID` | Integer | Auto-incremented unique identifier for each report |
| `Type` | String | `Lost` or `Found` |
| `Item Name` | String | Title or name of the item (e.g., iPhone 13, Wallet) |
| `Category` | String | `Electronics`, `Personal Belongings`, `Clothing`, `Documents/Cards`, `Keys`, or `Other` |
| `Location` | String | Specific area or building where the item was lost or found |
| `Date` | Datetime String | Timestamp of report creation (`YYYY-MM-DD HH:MM`) |
| `Description` | String | Color, brand, distinguishing features, etc. |
| `Contact Info` | String | Contact email or phone number for claimant/finder |
| `Status` | String | Item resolution status (`Open` or `Claimed/Resolved`) |

---

## 🛠️ Tech Stack & Requirements

- **Language**: Python 3.8+
- **Data Manipulation**: [pandas](https://pandas.pydata.org/)
- **UI & Widgets**: [ipywidgets](https://ipywidgets.readthedocs.io/)
- **Runtime Environment**: [Google Colab](https://colab.research.google.com/) or [Jupyter Notebook / JupyterLab](https://jupyter.org/)

---

## ⚡ Quick Start

### Option 1: Run in Google Colab (Fastest)

Click the badge below to directly open and run the notebook in your browser with zero setup:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Anshul-lite/digital-lost-and-found-system/blob/main/digital_lost_and_found_system.ipynb)

1. Click **Runtime** > **Run all** (or press `Ctrl + F9`).
2. The interactive UI will appear at the bottom of the second cell.

---

### Option 2: Run Locally on Your Machine

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Anshul-lite/digital-lost-and-found-system.git
   cd digital-lost-and-found-system
   ```

2. **(Optional) Set up a virtual environment**:
   ```bash
   # Windows
   python -m venv venv
   .\venv\Scripts\activate

   # macOS / Linux
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter**:
   ```bash
   jupyter notebook digital_lost_and_found_system.ipynb
   ```
   *or with JupyterLab:*
   ```bash
   jupyter lab digital_lost_and_found_system.ipynb
   ```

5. **Run the notebook cells** to start using the system.

---

## 🖥️ User Interface Overview

```text
=== DIGITAL LOST AND FOUND SYSTEM ===
[ Report Item ] [ Search Database ] [ Resolve/Claim ]
────────────────────────────────────────────────────────
Type:        [ Lost / Found ▼ ]
Item Name:   [ e.g., iPhone 13, Leather Wallet ]
Category:    [ Electronics ▼ ]
Location:    [ e.g., Library 2nd Floor ]
Description: [ Color, brand, distinguishing features... ]
Contact:     [ Email or Phone Number ]
             [  Submit Report  ]
```

---

## 📂 Project Structure

```text
digital-lost-and-found-system/
│
├── digital_lost_and_found_system.ipynb   # Main interactive notebook application
├── requirements.txt                      # Project dependencies
├── .gitignore                            # Git ignore rules for Python & Jupyter
└── README.md                             # Project documentation
```

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
Feel free to check out the [issues page](https://github.com/Anshul-lite/digital-lost-and-found-system/issues).

---

## 👤 Author

- **Anshul Gour**
- GitHub: [@Anshul-lite](https://github.com/Anshul-lite)
- Email: [anshulgour074@gmail.com](mailto:anshulgour074@gmail.com)
