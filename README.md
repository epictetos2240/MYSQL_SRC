## 리눅스에 MYSQL 설치하기

URL 주소 = https://apost.dev/sql-ubuntu-mysql-seolci-mic-hwangyeong-seoljeong/


sudo apt update   
sudo apt install mysql-server   
sudo ufw allow mysql

sudo systemctl start mysql   
sudo systemctl enable mysql

sudo mysql -u root   

create database  **madangdb** ;  
create user **madang**@localhost identified by '**madang**';   
grant all privileges on **madangdb**. * to **madang**@localhost;   
commit;


## 리눅스에 MYSQL 삭제하기

URL 주소 = https://2vup.com/ubuntu-remove-mysql/

우분투에서 MYSQL 완전 삭제   
sudo apt-get remove ---purge mysql*   

mysql 관련 파일들 리스트 확인   
sudo apt -get remove --purge **madang** 

sudo rm -rf /etc/mysql /var/lib/mysql   
sudo rm -rf /var/log/mysql   
sudo rm -rf /var/log/mysql.*    
sudo rm /var/lib/dpkg/info/*   
sudo apt-get autoremove   
sudo apt-get autoclean   









