# MAGiC Genetic Circuit Simulator

A Flask-based web app for designing and simulating genetic circuits.

---

## Prerequisites

1. **Python 3.8 or newer**  
   - Download and install from [python.org](https://www.python.org/downloads/).  
   - Make sure to **check “Add Python to PATH”** on Windows.

2. **Visual Studio Code (VS Code)**  
   - Download from https://code.visualstudio.com/  
   - Install the **Python** extension (look for “ms-python.python”).

---

1. Create & Activate a Virtual Environment

Keeping your project dependencies isolated is best practice.

Windows (PowerShell)
python -m venv .venv
.\.venv\Scripts\Activate.ps1

If you get a policy error, run Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser in PowerShell as administrator.

macOS/Linux
python3 -m venv .venv
source .venv/bin/activate

2. Install Dependencies
With your virtual environment activated, install the required packages:
pip install --upgrade pip
pip install flask flask-cors numpy scipy matplotlib

Alternatively, you can use requirements.txt, just run:

pip install -r requirements.txt

3. Open the Project in VS Code
Launch VS Code.

File → Open Folder… and select the project folder.

In the bottom-left corner, click the Python version and choose the interpreter from ./.venv.

You should now have syntax highlighting and IntelliSense for Python.

4. Run the Application
In VS Code’s terminal (which should already be using your virtual env), run:
   python app.py
You should see output like:
 * Running on http://127.0.0.1:3000/ (Press CTRL+C to quit)

5. View in Your Browser
Open your browser and go to:
http://127.0.0.1:3000/

6. Common Troubleshooting
“Module not found” errors
Make sure your virtual environment is activated (.venv\Scripts\activate on Windows or source .venv/bin/activate on macOS/Linux).

Port 3000 already in use
Stop any other process using port 3000 or edit app.run(port=…) in app.py.

CSS or images not loading
Ensure your static/ folder contains your .css and image files, and that your Flask app is configured with static_folder='static'.

8. Next Steps
Explore templates/ for the HTML files (loading.html, index.html, etc.).

Tweak the simulation logic in app.py under run_simulation().

Have fun building and simulating your own genetic circuits!

Happy Gene Modeling!
– The MAGiC Team


