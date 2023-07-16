# tools
It is a reference to POC-CVE-2023-32233 , i was seeing that is was made for ubuntu 23
I was modifing the source and test it in a centos 8.
stuff to do or need it :
sudo yum install libmnl-devel libnftnl-devel -y

sudo yum install epel-release -y

sudo yum groupinstall "Development Tools" -y

sudo update -y

gcc -Wall -o exploit exploit.c -lmnl -lnftnl -lpthread

./exploit

If only want to test it y upload it the compilated source for centos 
and also for ubuntu(was compilated in a Ubuntu 22.02).

Test it if centos with ./centos

if Ubuntu with ./ubuntu 
