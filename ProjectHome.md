Use this python script to automate any Cisco IOS CLI Commands.

# Example #
```
# Test.py
from Router import Router
hostname = 'router1'
R1 = Router(hostname, logfile='Log.log')
login_cmd = 'telnet router1'
username = 'uname'
password = 'pwd'
login_expect = hostname + '#'
R1.login(login_cmd, username, password, login_expect)
print repr(R1.exec_cmd('show clock'))
R1.logout()
```

# FAQs #
Ask wilson.amit@gmail.com