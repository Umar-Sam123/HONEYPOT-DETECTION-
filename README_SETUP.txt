HONEYGUARD AI - DJANGO HONEYPOT PROJECT

1. Open Anaconda Prompt / Command Prompt.
2. cd /d C:\Users\Umar\Desktop\HoneypotAttack
3. (Recommended) create an environment:
   conda create -n honeypot python=3.11 -y
   conda activate honeypot
4. Install packages:
   python -m pip install -r requirements.txt
5. Run migrations:
   python manage.py migrate
6. Optional: create an admin account:
   python manage.py createsuperuser
7. Start:
   python manage.py runserver
8. Open:
   http://127.0.0.1:8000/

Main pages:
Home       /
Register   /register/
Login      /login/
Predict    /data/
Result     /predict/
Admin      /adminlogin/
Dashboard  /adminhome/
About      /contact/

The project stores prediction events in db.sqlite3.
The ML model is trained once per server process from the bundled CSV and
uses consistent preprocessing with unknown-category handling.
