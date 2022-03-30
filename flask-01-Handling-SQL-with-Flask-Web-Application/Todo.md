
## Installations
- Front-End Sides
    - VSCode
        - Extension 
            {
                - KnisterPeter.vscode-github
                - GitHub.vscode-pull-request-github
                - GitHub.vscode-pull-request-github
                - formulahendry.vscode-mysql
                - jakebathman.mysql-syntax
                - slightc.pip-manager
                - etmoffat.pip-packages
                - ms-python.python
                - ms-vscode-remote.remote-ssh
                - ms-vscode-remote.remote-ssh-edit
            }
        - Pip Manager
            {
                Flask
                Flask-MySQL
                PyMySQL
            }
    - Windows 10X
        - MySQL WorkBench
        - Git
- Back-End Side
    - AWS RDS (with MYSql instance HTTP + MYSQL SecGroup AnyWhere)
    - EC2 (Linux 2 AMI instance HTTP + SSH SecGroup AnyWhere)
        - Flask
        - Flask-MySQL
        - PytHon
        - SSH (Move project folder (.html, .py ) with Remote Explorer updating .ssh config file)

## To Do AWS EC2
    - Connect using VScode Remote Explorer Tab
        -   Configure config File below
                Host BLaBla ( please any Server Name viewing your VSCode Remote Explorer)
                    HostName 54.166.57.173 (please input your EC2 Linux AMI Public IP Adress)
                     IdentityFile ...pem (please inpu your .pem file using the path)
                     User ec2-user (your EC2 user name)
                Host *
                TCPKeepAlive yes
                ServerAliveInterval 120
        -   Checking the load packages and loading what you need over EC2 Linux AMI 
            (You must be connected using SSH via vscode)
            - Choose SSH Targets over VSCode Remote Explorer Tab and see your EC2 insance then select folder
            - create folder its name Flask and move template folder including .html file and .py files
            - Open new terminal EC2 instance using VSCode-->New Terminal --> set Git
            - Write below
                - sudo yum update -y
                - pip3 install flask
                - pip3 install Flask-MySQL
                - pip3 install PyMySQL
                - python3 app-with-mysql.py (for viewing EC2 Linux AMI over any webpage locally)
                - pip3 install flask_mysql
                - set app-with-mysql.py app.run(host='0.0.0.0', port=80) (for viewing EC2 Linux AMI over any   webpage anywhere in-oubound)








            
