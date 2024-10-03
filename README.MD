Java Based tool with many plugins for CI/CD.
Open Source Stand Alone Automation Server.

Architecture:

Different Developers following CI
👇
GithubRepo🗃️ -> <- Jenkins Server (Automation Tool) 🗜️🖥️ -> Selenium -> Deploy

Master - Salve Architecture
1 - M
Build/Execution is done using slaves (Windows, Mac, Linux)

create virtual environment using
`python -m venv .venv`

source this environment
`Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process`
`.\.venv\Scripts\Activate.ps1`

install all the dependencies
`pip install -r requirements.txt`

Test the application
`pytest test.py`
