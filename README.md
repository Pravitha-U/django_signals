# Django Signals - User Creation & Deletion  

## Overview  
This project demonstrates Django *signals* to track user creation and deletion events.  

## Steps to Run  

1. *Clone the Repository*  
   ```sh
   git clone <your-repo-url>
   cd <your-project-folder>

2. Setup Virtual Environment & Install Dependencies

python -m venv venv  
source venv/bin/activate  # On Windows: venv\Scripts\activate  
pip install -r requirements.txt


3. Run Migrations & Start Server

python manage.py migrate  
python manage.py runserver


4. Test in Django Shell

python manage.py shell

Create User

from django.contrib.auth.models import User  
user = User.objects.create(username="testuser")

Delete User

user.delete()




Expected Output

User Created: testuser

User Deleted: testuser


Files Modified

apps.py → Connects signals

signals.py → Defines user tracking



---
