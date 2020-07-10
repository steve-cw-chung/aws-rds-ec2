# aws-rds-ec2

1. Create ec2 from aws
2. Create a key pair and save it at the secured place
3. Change the permission for the key pair and remove the inheritance
4. Use ssh to connect

Jupyter Notebook
use yum instead of apt-get in amazon linux2

Need to install python3 if not installed previously
0. python --version
0.1. sudo yum install python37
0.2. python3 --version
0.3. curl -O https://bootstrap.pypa.io/get-pip.py
0.4. python3 get.pip.py --user
0.5. pip --version
0.6. pip install awsebcli --upgrade --user
0.7. eb --version 
1. sudo apt-get update 
2. sudo apt-get install python3-pip
3. sudo pip3 install notebook
4. python3
5. from notebook.auth import passwd
6. passwd()
7. enter password
8. copy the hash key including the 'hash'
9. quit()
10. jupyter notebook --generate-config
11. sudo vi /home/../.jupyter/jupyter_notebook_config.py
12. go to the end of the file
13. press a
14. c = get_config()
15. c.NotebookApp.password = u'hash'
16. c.NotebookApp.ip = 'ip'
17. :wq
18. jupyter-notebook --allow-root
19. control-z
20. Go to security group and add to inbound the 8888 custom TCP 
21. ip:8888
22. enter password
23. control-z
24. bg
25. disown -h

