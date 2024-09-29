Deploying the web application in AWS. the Book Management App is a simple web application designed for users to add, view, and delete books. With a clean and intuitive interface, users can input the title, author, and description of each book, showcasing basic functionality in JavaScript, DOM manipulation, and event handling.

Step to run on AWS 
->Transfer Files to EC2:
      ->Use scp (secure copy) to transfer files. Replace your-key.pem, /path/to/local/file, and ec2-user@your-ec2-instance-public-dns accordingly:
              scp -i "your-key.pem" /path/to/local/file ec2-user@your-ec2-instance-public-dns:/path/on/ec2
      ->To transfer a directory, use:
              scp -i "your-key.pem" -r /path/to/local/directory ec2-user@your-ec2-instance-public-dns:/path/on/ec2

Step to run in LINUX:
    sudo su -,
    yum install -y httpd,
    mkdir temp,
    cd temp,
    exit,
    sudo mv zip file name /root/tmep/,
    sudo su -,
    cd temp,
    unzip zip file name,
    cd complex,
    ls -lrt,
    mv * /var/www/html,
    systemctl enable httpd,
    systemctl start httpd,
    systemctl status httpd  // Active part should be in running state.
    
