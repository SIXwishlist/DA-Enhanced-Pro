# DA-Enhanced-Pro
DA-Enhanced-Pro - Free DirectAdmin Skin by dugalex

If installed as "enhanced" skin, it will be automatically updated on DirectAdmin updates and will retain it's original design.  
All colors on the top left and right are available. To change a color click on the desired color box. 

![Admin](https://github.com/dugalex/DA-Enhanced-Pro/blob/master/images/skin-admin.jpg)
![Reseller](https://github.com/dugalex/DA-Enhanced-Pro/blob/master/images/skin-reseller.jpg)
![User](https://github.com/dugalex/DA-Enhanced-Pro/blob/master/images/skin-user.jpg)


<b>Installation:</b>

--------------------------------------------------------------------
!!!WARNING!!! This will change the default "enhanced" skin but will not overwrite any existing DirectAdmin files.
--------------------------------------------------------------------

cd /usr/local/directadmin/data/skins/  
wget https://github.com/dugalex/DA-Enhanced-Pro/archive/master.zip  
unzip master.zip  
cd DA-Enhanced-Pro-master  
cp -rn * ../enhanced  
cd ..
chown -R diradmin:diradmin enhanced  
rm -rf DA-Enhanced-Pro-master  
rm -f master.zip  
exit  

--------------------------------------------------------------------
!!! OR !!!
--------------------------------------------------------------------  
This will not change the default "enhanced" skin. It will create a new "enhanced-pro" skin.  
You will have to manually copy and overwrite the files from "enhanced" skin after directadmin update.  

--------------------------------------------------------------------

cd /usr/local/directadmin/data/skins/  
wget https://github.com/dugalex/DA-Enhanced-Pro/archive/master.zip  
unzip master.zip  
mv DA-Enhanced-Pro-master enhanced-pro  
chown -R diradmin:diradmin enhanced-pro  
rm -f master.zip  
exit 
