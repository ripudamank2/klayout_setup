# klayout_setup
# Install the dependent packages for Klayout 
sudo apt-get insatll python3 python3-dev ruby ruby-dev build-essential libz-dev git
Search package ---> apt-cache search <package_name> 
libqt<latest_version>-dev-bin libqt<latest_version>-dev

---------------------------------------------------------------------- \
Command : git clone <git_address> <directory>   \ 
git clone https://github.com/klayoutmatthias/klayout klayout  \
cd klayout  \
git checkout 0.26   \
-----------------------  \
# Change the permission of build.sh  \
 
$chmod u+x build.sh
-------------below command will take utpo 3hrs or less--------
$./build.sh

--------------change the permission of excecutable binary--------
$ chmod u+x bin-release/klayout

--------------In your Klayout directory-----------------------
Create a file with the name Klayout using any editor and add the below line 
vim klayout
export PATH=$<path to location>/.klayout/bin-release:$PATH
export LD_LIBRARY_PATH=$<path to location>/.klayout/bin-release:$LD_LIBRARY_PATH
klayout -e
--------------------------------------------------------------------
# In .bashrc put the path of the klayout file which you had created
 export PATH='"'$<path to location>/.klayout:$PATH 
 $source .bashrc 
  
  Finish Installation
