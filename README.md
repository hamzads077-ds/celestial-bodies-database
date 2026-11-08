# 🌌 Celestial Bodies Database

A PostgreSQL relational database designed and implemented as part of the **freeCodeCamp Relational Database Certification**. The project models a astronomical structure containing galaxies, stars, planets, moons, and galaxy types with strict relational integrity, custom constraints, and foreign key mappings.

---

## 🛠️ Tech Stack & Database System
* **Database Engine:** PostgreSQL
* **Tooling:** `psql`, Dev Containers, Bash Shell
* **Version Control:** Git, GitHub

---

## 📐 Database Schema & Architecture

The database `universe` consists of 5 interconnected tables:

1. **`galaxy`**: Stores information about galaxies (e.g., Milky Way, Andromeda).
2. **`star`**: Contains star data linked directly to a parent galaxy via foreign key (`galaxy_id`).
3. **`planet`**: Stores planetary details linked to a parent star via foreign key (`star_id`).
4. **`moon`**: Contains natural satellites linked to a parent planet via foreign key (`planet_id`).
5. **`galaxy_types`**: A lookup table defining structural classifications of galaxies.

---

## ✨ Features & Constraints
* **Primary & Foreign Keys:** Automated auto-incrementing `SERIAL` primary keys across all tables alongside parent-child foreign key cascades.
* **Data Integrity:** String columns (`VARCHAR`, `TEXT`), Numeric types (`INT`, `NUMERIC`), and Boolean constraints (`NOT NULL`, `UNIQUE`).
* **Complete Dataset:** Populated with multi-row records meeting all automated validation checks.

---

## 📜 Course Link

This project is part of the official curriculum:
- 🎓 **Course**: [![freeCodeCamp](https://img.shields.io/badge/freeCodeCamp-0a0a23?style=for-the-badge&logo=freecodecamp&logoColor=white)](https://www.freecodecamp.org/learn/relational-database/)
