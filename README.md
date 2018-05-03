Mihika Naik
Arianne Silvestre 

Here are the commands to build the motivity project in Linux. I have used Ubuntu 16.04 its and this was the only OS and version the framework worked on for me. 
sudo rm /var/lib/apt/lists/lock
sudo rm /var/cache/apt/archives/lock
sudo rm /var/lib/dpkg/lock
sudo apt-get install git-core
sudo apt-get install scons
sudo apt-get install ssh
sudo apt-get install build-essential g++
sudo apt-get install libboost-dev libboost-program-options-dev lib
cd
ls
tar xzvf boost_1_55_0.tar.gz
cd boost_1_55_0/
./bootstrap.sh --with-libraries=system,filesystem,date_time,thread,regex,log,iostreams,program_options --prefix=/usr/local
sudo apt-get update
sudo apt-get install python-dev autotools-dev libicu-dev build-essential libbz2-dev
sudo ./b2 install
sudo sh -c 'echo '/usr/local/lib' >> /etc/ld.so.conf.d/local.conf'
sudo ldconfig
udo apt-get install doxygen
cd iotivity-1.3.1/
scons
git clone https://github.com/01org/tinycbor.git extlibs/tinycbor/tinycbor -b v0.4.1
scons
git clone https://github.com/ARMmbed/mbedtls.git extlibs/mbedtls/mbedtls -b mbedtls-2.4.2
scons
sudo apt-get install sqlite3 libsqlite3-dev
scons
cd resource/examples/release
./simpleserver
./simpleserver.cpp
./simpleserver
./simpleserver.cpp
chmod u+x simpleserver.cpp
./simpleserver.cpp
cd out/linux/x86_64/release/resource/examples/
./simpleserver


