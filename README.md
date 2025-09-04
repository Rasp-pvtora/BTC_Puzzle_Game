# 📜 BTC-Puzzle Export Script – Overview
An **open source Bitcoin script**. Use the bruteforce random to crack the BTC puzzle game.

Do you like this work? why don't you buy me a coffee?
₿ = 000000000

# 🎯 Objective
This script automates the process of finding solutions to the btc puzzle and creates organized CSV exports with all tested keys and addresses, along with the solution (if) found.
It is designed to run as a Tampermonkey UserScript, so it runs directly in your browser without needing to install additional software.

# 🔧 Main Features
- **Controlled Start and Stop:**
    - Adds two buttons to the page: Start Script and Stop Script.
    - The user can choose which puzzle level to start from.
    - The script automatically moves on to the next puzzle once a solution is found.

- **Automatic Field Population:**
    - Automatically fills in the Start HEX, End HEX, Target Address, and Max. Keys fields based on the selected puzzle.

- **Automated Search Loop:**
    - Simulates clicks on the Random button to generate and test new keys.
    - Collects all results from the table shown on the site.
    - Keeps track of the number of clicks performed.

- **Data Export:**
    - Automatically exports a CSV file containing all tested keys and their corresponding addresses.
    - If the correct solution is found, the CSV file includes both the winning key and all keys tested up to that point.
    - When the maximum number of clicks (clickCount) is reached, partial results are saved, and the script automatically restarts on the same puzzle.

- **Automatic Puzzle Switching:**
    - When a solution is found, the script exports the results and automatically moves to the next puzzle.
    - It continues working until the end of the puzzle list is reached.

- **Robustness:**
    - If the fields are not filled in correctly on the first attempt, the script retries multiple times.
    - Manages the case where the key has already been found and is shown on the page.
    - Prevents duplicate exports with an internal flag (solutionExported).

# 📂 Output
Files are automatically saved as CSVs, with names like:

- **btcpuzzle_scan_YYYYMMDD_HHMM.csv** → for partial scans.
- **btcpuzzleXX_solution_YYYYMMDD_HHMM.csv** → for solved puzzles (XX = puzzle number).

# 👤 Practical Use

1. The user opens the XXXXX page.
2. The user starts the script by clicking Start Script.
3. The script then automatically handles the entire process:
    🔹 Entering parameters
    🔹 Automatic scanning
    🔹 Saving to CSV
    🔹 Moving on to the next puzzle

## 🔥 I also offer advanced courses, one-to-one personalized coaching, project job offers. 
Interested? Than schedule an appointment: **✉️ Contact [EMAIL NOT EXISTING](mailto:info@gmail.com)**

## 🚀 Projects & Contributions
This GitHub profile will host a variety of **open-source projects and security resources**, including:
- 🔹 **Security tools** and Automated Web/Cloud tools.
- 🔹 **Script injection or Script dev** and proof-of-concept (PoC) code.
- 🔹 **Microcontroller software** for Raspberry Pi, Arduino, and home automation experiments.

## 🛠️ Contributing
I welcome contributions from the community! If you’d like to contribute:
1. **Fork the repository** and make your changes.
2. **Create a pull request** with a detailed description of your changes.
3. **Ensure your code follows best practices** and is well-documented.
4. **Engage in discussions** to improve and refine security tools and research.

## 📜 License
Most of our projects are released under the **MIT License**, unless stated otherwise in the repository. See individual repositories for license details.
