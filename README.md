## Programmer Assessment Q4

This repository contains a broken web app built with Dash. Please follow the tasks below.

Tasks:
1. Clone this repo to your machine.
2. Fix missing dependencies and fill authors section in `pyproject.toml`.
3. Fix bugs prevent the app `main.py` from running.
4. Change port the app ruuning on to `10030`.
5. Commit you changes.
6. Update `README.md` with a instruction
   1. Assuming the user has a fresh minimum Linux installation with no python.
   2. Setup python and virtual environment for this app, remember to use the fixed `pyproject.toml`.
   3. How to run this app and how to access it without portforwarding.
7. Push all the changes to your own repository on Github, and provide a link to your own repo in your submission in the last.


## 6. Instruction

How to set up and run the app on a fresh Linux installation:

### System Setup
1. Update your package list:
   ```
   sudo apt update
2. Install Python 3.11, pip, and git
   ```
   sudo apt install -y python3.11 python3.11-venv python3-pip git
3. Clone the repository
   ```
   git clone <https://github.com/katherinerbanis/Assessment-debugging>
   cd debugging-q4
4. Create and Activate Virtual Environment
   ```
   python3.11 -m venv venv
   source venv/bin/activate
5. Install Dependencies
   ```
   pip install .
6. Run the app
   ```
   python main.py
   ```
### Accessing the app
#### On the same machine
   ```
   http://127.0.0.1:10030
   ```

#### On another device on the same local network:
1. First run the app with:
   ```
   app.run_server(debug=True, port=10030, host="0.0.0.0")
   ```
2. Then open in your browser:
   ```
   http://<your-linux-ip>:10030
   ```
   Note: Replace <your-linux-ip> with the actual IP address of your Linux machine. You can find it by running:
   ```
   hostname -I
   ```
