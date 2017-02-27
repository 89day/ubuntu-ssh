# ubuntu-ssh
Base Ubuntu system with OpenSSH-server

    user:root
    password:password

1、Creat a ubuntu-ssh folder，for store any files will use

    cd /
    mkdir ubuntu-ssh
    cd ubuntu-ssh
    touch start.sh
    touch Dockerfile

2、Edit start.sh
3、Edit Dockerfile
4、Build Docker image

    sudo docker build -t 89day/ubuntu-ssh .
    #Here is a . in the end    

5、Run the image and test

    sudo docker run -d -p 32800:22 89day/ubuntu-ssh
    #32800:22 Maps a ssh port to a network resource
