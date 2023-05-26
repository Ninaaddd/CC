id: vagrant
password: vagrant
*whenever asked*

VM1:
touch abc.txt
cat abc.txt
nano abc.txt
*ctrl+x*
*enter*

VM2:
ifconfig
*note the ip down*

VM1:
scp abc.txt vagrant@<ip_address>:/home/vagrant
*say yes*
*enter password*

VM2:
ls
cat abc.txt