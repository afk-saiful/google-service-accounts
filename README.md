# google-service-accounts

``
Steps
``
- pip3 install -r requirements.txt
- python gen_sa_accounts.py
- python gen_sa_accounts.py --list-projects
- python gen_sa_accounts.py --enable-services projectid | ``Change projectid with your project id``
- python gen_sa_accounts.py --create-sas projectid | ``Change projectid with your project id``
- python gen_sa_accounts.py --download-key projectid | ``Change projectid with your project id``

accounts folder --> powershell

```
$emails = Get-ChildItem .\**.json |Get-Content -Raw |ConvertFrom-Json |Select -ExpandProperty client_email >>emails.txt
```