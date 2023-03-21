Instructions to Make Dockerfile using website 

wget https://www.tooplate.com/zip-templates/2132_clean_work.zip
#use wget to install the website 
sudo apt install unzip
#install unzip to Unzip the file and change to TAR 
unzip 2132_clean_work.zip

tar czvf nano.tar.gz *
#tar the website files 

vim Dockerfile
#write the Dockerfile
Docker build -t nanoimage:v1 .
#Build
 docker run --name nano -d -P nanosite:v1

curl ifconfig.me
#get the public IP of the EC2 
