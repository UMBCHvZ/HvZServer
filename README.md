# HvZServer
UMBC HvZ's main server code.

# Setup
First, ensure you have the latest version of Python 3 installed: https://www.python.org/downloads/ 

# PyCharm setup
1. Open PyCharm.
2. Click `Check out from Version Control`, and put in `https://github.com/UMBCHvZ/HvZServer.git` as the URL.
3. Pick somewhere to put it locally.
4. Click `Clone`.
5. When it says this is a PyCharm project, say you want to open it.
6. There should be a file list on the left; if not, go to View->Tool Windows->Project.
7. Open manage.py; you should get a yellow banner across the top.
8. Click `Configure Python interpreter`.
9. Click the gear in the top right, then "Add..."
10. Make sure "Virtualenv Environment" is selected on the left; leave all the defaults, and click `OK`.
11. Let it finish doing what it's doing, this might take a minute.
12. Click "OK" again, and ignore it complaining about packaging tools if it shows up.
13. There should still be a yellow banner across the top. Click `Install requirements`.
14. Click `Install`.
15. Let it sit for a while, this isn't fast; you can see the progress bar at the bottom.
16. Go to `Run`->`Edit Configurations`
17. Click the green + in the top left, and choose Django Server.
18. Name the configuration something reasonable ("Run server"), and click OK.
19. In the top right, click the Play button.
20. Go to [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

# Command line setup
First, clone this repo using the method of your choice. Then, open a command prompt in the root of the repo, and run:
```
pip install virtualenv
virtualenv venv
venv\Scripts\activate.bat
pip install -r requirements.txt
python manage.py runserver 8000
```
Then go to [http://127.0.0.1:8000/](http://127.0.0.1:8000/).