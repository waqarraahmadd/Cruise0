## Cruise0 Auth0 PoC

**Auth0 Tenant Name**: Shared via email


- Auth0 login integration via email/password and google social
- Blocking disposable emails via Pre-User Registration Action
- Email verification via link
- Custom login page with Cruise0 branding (logo + background)
- MFA for non-social only

## Setup & Run
1. Clone the repo:
```bash
git clone https://github.com/waqarraahmadd/Cruise0.git
cd Cruise0
```

2. Create and activate a Python virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate   # Mac/Linux
```

3. Install dependencies (or via packages in UI if using Pycharm):
```bash
pip install -r requirements.txt
```

4. Configure `.env` with your Auth0 credentials. Should be able to get that from my account. Tenant shared above.

5. Run the app:
```bash
python server.py
```

6. Open browser at: `http://localhost:3000`

## Notes
- Disposable emails are blocked on signup via disify API.  
- Login page uses Cruise0 logo and background.  
- Pre-User Registration Action handles disposable email validation.
