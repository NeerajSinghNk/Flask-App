Whoami:~$ mkdir myApp
Whoami:~$ cd myApp
Whoami:~/myApp$ python3 -m venv venv
Whoami:~/myApp$ . venv/bin/activate
(venv) Whoami:~/myApp$ pip install Flask
Collecting Flask
  Using cached https://files.pythonhosted.org/packages/f2/28/2a03252dfb9ebf377f40fba6a7841b47083260bf8bd8e737b0c6952df83f/Flask-1.1.2-py2.py3-none-any.whl
Collecting Werkzeug>=0.15 (from Flask)
  Using cached https://files.pythonhosted.org/packages/cc/94/5f7079a0e00bd6863ef8f1da638721e9da21e5bacee597595b318f71d62e/Werkzeug-1.0.1-py2.py3-none-any.whl
Collecting itsdangerous>=0.24 (from Flask)
  Using cached https://files.pythonhosted.org/packages/76/ae/44b03b253d6fade317f32c24d100b3b35c2239807046a4c953c7b89fa49e/itsdangerous-1.1.0-py2.py3-none-any.whl
Collecting Jinja2>=2.10.1 (from Flask)
  Using cached https://files.pythonhosted.org/packages/30/9e/f663a2aa66a09d838042ae1a2c5659828bb9b41ea3a6efa20a20fd92b121/Jinja2-2.11.2-py2.py3-none-any.whl
Collecting click>=5.1 (from Flask)
  Using cached https://files.pythonhosted.org/packages/dd/c0/4d8f43a9b16e289f36478422031b8a63b54b6ac3b1ba605d602f10dd54d6/click-7.1.1-py2.py3-none-any.whl
Collecting MarkupSafe>=0.23 (from Jinja2>=2.10.1->Flask)
  Using cached https://files.pythonhosted.org/packages/b2/5f/23e0023be6bb885d00ffbefad2942bc51a620328ee910f64abe5a8d18dd1/MarkupSafe-1.1.1-cp36-cp36m-manylinux1_x86_64.whl
Installing collected packages: Werkzeug, itsdangerous, MarkupSafe, Jinja2, click, Flask
Successfully installed Flask-1.1.2 Jinja2-2.11.2 MarkupSafe-1.1.1 Werkzeug-1.0.1 click-7.1.1 itsdangerous-1.1.0
(venv) Whoami:~/myApp$ pip install -U https://github.com/pallets/flask/archive/master.tar.gz
Collecting https://github.com/pallets/flask/archive/master.tar.gz
  Downloading https://github.com/pallets/flask/archive/master.tar.gz
     | 768kB 178kB/s
Requirement already up-to-date: Jinja2>=2.10.1 in ./venv/lib/python3.6/site-packages (from Flask==2.0.0.dev0)
Requirement already up-to-date: Werkzeug>=0.15 in ./venv/lib/python3.6/site-packages (from Flask==2.0.0.dev0)
Requirement already up-to-date: click>=5.1 in ./venv/lib/python3.6/site-packages (from Flask==2.0.0.dev0)
Requirement already up-to-date: itsdangerous>=0.24 in ./venv/lib/python3.6/site-packages (from Flask==2.0.0.dev0)
Requirement already up-to-date: MarkupSafe>=0.23 in ./venv/lib/python3.6/site-packages (from Jinja2>=2.10.1->Flask==2.0.0.dev0)
Installing collected packages: Flask
  Found existing installation: Flask 1.1.2
    Uninstalling Flask-1.1.2:
      Successfully uninstalled Flask-1.1.2
  Running setup.py install for Flask ... done
Successfully installed Flask-2.0.0.dev0
(venv) Whoami:~/myApp$ sudo apt-get install python-virtualenv
[sudo] password for neeraj: 
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages were automatically installed and are no longer required:
  linux-headers-5.3.0-28 linux-headers-5.3.0-28-generic linux-headers-5.3.0-40
  linux-headers-5.3.0-40-generic linux-image-5.3.0-28-generic
  linux-image-5.3.0-40-generic linux-modules-5.3.0-28-generic
  linux-modules-5.3.0-40-generic linux-modules-extra-5.3.0-28-generic
  linux-modules-extra-5.3.0-40-generic
Use 'sudo apt autoremove' to remove them.
The following additional packages will be installed:
  python3-virtualenv virtualenv
The following NEW packages will be installed:
  python-virtualenv python3-virtualenv virtualenv
0 upgraded, 3 newly installed, 0 to remove and 11 not upgraded.
Need to get 94.6 kB of archives.
After this operation, 316 kB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://in.archive.ubuntu.com/ubuntu bionic/universe amd64 python-virtualenv all 15.1.0+ds-1.1 [46.8 kB]
Get:2 http://in.archive.ubuntu.com/ubuntu bionic/universe amd64 python3-virtualenv all 15.1.0+ds-1.1 [43.4 kB]
Get:3 http://in.archive.ubuntu.com/ubuntu bionic/universe amd64 virtualenv all 15.1.0+ds-1.1 [4,476 B]
Fetched 94.6 kB in 3s (33.3 kB/s)     
Selecting previously unselected package python-virtualenv.
(Reading database ... 261211 files and directories currently installed.)
Preparing to unpack .../python-virtualenv_15.1.0+ds-1.1_all.deb ...
Unpacking python-virtualenv (15.1.0+ds-1.1) ...
Selecting previously unselected package python3-virtualenv.
Preparing to unpack .../python3-virtualenv_15.1.0+ds-1.1_all.deb ...
Unpacking python3-virtualenv (15.1.0+ds-1.1) ...
Selecting previously unselected package virtualenv.
Preparing to unpack .../virtualenv_15.1.0+ds-1.1_all.deb ...
Unpacking virtualenv (15.1.0+ds-1.1) ...
Setting up python3-virtualenv (15.1.0+ds-1.1) ...
Setting up python-virtualenv (15.1.0+ds-1.1) ...
Setting up virtualenv (15.1.0+ds-1.1) ...
Processing triggers for man-db (2.8.3-2ubuntu0.1) ...
(venv) Whoami:~/myApp$ pip install flask-sqlalchemy
Collecting flask-sqlalchemy
  Downloading https://files.pythonhosted.org/packages/1e/65/226d95466c75e34e291a76890ed0e27af2e46ab913002847856f11d4d59d/Flask_SQLAlchemy-2.4.1-py2.py3-none-any.whl
Collecting SQLAlchemy>=0.8.0 (from flask-sqlalchemy)
  Downloading https://files.pythonhosted.org/packages/96/4c/35fccaa5a642f7f4f887798662fefb21b8366c429f3ce4c59c7b077811b4/SQLAlchemy-1.3.16-cp36-cp36m-manylinux1_x86_64.whl (1.2MB)
    100% |████████████████████████████████| 1.2MB 236kB/s 
Requirement already satisfied: Flask>=0.10 in ./venv/lib/python3.6/site-packages (from flask-sqlalchemy)
Requirement already satisfied: Jinja2>=2.10.1 in ./venv/lib/python3.6/site-packages (from Flask>=0.10->flask-sqlalchemy)
Requirement already satisfied: Werkzeug>=0.15 in ./venv/lib/python3.6/site-packages (from Flask>=0.10->flask-sqlalchemy)
Requirement already satisfied: click>=5.1 in ./venv/lib/python3.6/site-packages (from Flask>=0.10->flask-sqlalchemy)
Requirement already satisfied: itsdangerous>=0.24 in ./venv/lib/python3.6/site-packages (from Flask>=0.10->flask-sqlalchemy)
Requirement already satisfied: MarkupSafe>=0.23 in ./venv/lib/python3.6/site-packages (from Jinja2>=2.10.1->Flask>=0.10->flask-sqlalchemy)
Installing collected packages: SQLAlchemy, flask-sqlalchemy
Successfully installed SQLAlchemy-1.3.16 flask-sqlalchemy-2.4.1
(venv) Whoami:~/myApp$ pip install passlib
Collecting passlib
  Using cached https://files.pythonhosted.org/packages/11/b8/e9a78f3033228013ba8564adad8d0031bf9d39ea3acc3cdb9d55fabeb4ba/passlib-1.7.2-py2.py3-none-any.whl
Installing collected packages: passlib
Successfully installed passlib-1.7.2
(venv) Whoami:~/myApp$ code
(venv) Whoami:~/myApp$ pip install pymysql
Collecting pymysql
  Using cached https://files.pythonhosted.org/packages/ed/39/15045ae46f2a123019aa968dfcba0396c161c20f855f11dea6796bcaae95/PyMySQL-0.9.3-py2.py3-none-any.whl
Installing collected packages: pymysql
Successfully installed pymysql-0.9.3
(venv) Whoami:~/myApp$ pip install flask flask-login flask-wtf flask-sqlalchemy
Requirement already satisfied: flask in ./venv/lib/python3.6/site-packages
Collecting flask-login
  Downloading https://files.pythonhosted.org/packages/2b/83/ac5bf3279f969704fc1e63f050c50e10985e50fd340e6069ec7e09df5442/Flask_Login-0.5.0-py2.py3-none-any.whl
Collecting flask-wtf
  Using cached https://files.pythonhosted.org/packages/36/a9/8c01171066bd7a524ee005d81bb4a8aa446ab178043a1ad6cb5dc8f0bd83/Flask_WTF-0.14.3-py2.py3-none-any.whl
Requirement already satisfied: flask-sqlalchemy in ./venv/lib/python3.6/site-packages
Requirement already satisfied: Jinja2>=2.10.1 in ./venv/lib/python3.6/site-packages (from flask)
Requirement already satisfied: Werkzeug>=0.15 in ./venv/lib/python3.6/site-packages (from flask)
Requirement already satisfied: click>=5.1 in ./venv/lib/python3.6/site-packages (from flask)
Requirement already satisfied: itsdangerous>=0.24 in ./venv/lib/python3.6/site-packages (from flask)
Collecting WTForms (from flask-wtf)
  Using cached https://files.pythonhosted.org/packages/9f/c8/dac5dce9908df1d9d48ec0e26e2a250839fa36ea2c602cc4f85ccfeb5c65/WTForms-2.2.1-py2.py3-none-any.whl
Requirement already satisfied: SQLAlchemy>=0.8.0 in ./venv/lib/python3.6/site-packages (from flask-sqlalchemy)
Requirement already satisfied: MarkupSafe>=0.23 in ./venv/lib/python3.6/site-packages (from Jinja2>=2.10.1->flask)
Installing collected packages: flask-login, WTForms, flask-wtf
Successfully installed WTForms-2.2.1 flask-login-0.5.0 flask-wtf-0.14.3
(venv) Whoami:~/myApp$ 
