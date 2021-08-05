# python-cgi

Enable CGI in apache

1,Open Terminal and type 

apt-get update
apt-get install python3 python3-pip

2,sudo a2enmod cgi


service apache2 restart

3,cd /usr/lib/cgi-bin

4,vi /usr/lib/cgi-bin/test.py

5,#!/usr/bin/python3
from art import *
Art=text2art("TEST",font='block',chr_ignore=True)
print('Content-Type: text/plain')
print('')
print('This is my test!')
print(Art)

6,chmod 755 /usr/lib/cgi-bin/test.py

7,chmod 755 /usr/lib/cgi-bin/test.py
