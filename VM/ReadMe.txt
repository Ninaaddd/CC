Steps to Perform this practical
*Download vmdk image*
*create two virtual machines using this image*
*select vm1 under file tab under preferences choose network->nat network->add*
*repeat same procedure for vm2*
*then open vm1 first and follow the steps below*
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
