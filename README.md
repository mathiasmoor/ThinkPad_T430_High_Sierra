# ThinkPad_T430_High_Sierra
<i>Guide to run MAC OS X - High Sierra on Lenovo ThinkPad T430 laptop

Vanilla MAC OSX - High Sierra almost perfect on Lenovo T430.</i>
<br><br>

<code>Sources: ThiagoSchetini and RehabMan.</code>


<h1>Step by Step - GUIDE</h1>

<b>BIOS Settings : Turn SATA AHCI mode ON, UEFI Only Boot ON, Secure Boot OFF, CSM support OFF in UEFI settings. </b><hr>

<b>1. step - Create Bootable USB with High Sierra installator.</b> I think, the best choice for  creating USB installator is Olarila image from this links: https://drive.google.com/file/d/1XIeW2LCRZPSNq3_RiTvefAGIT_2fGfaW/view?usp=sharing
or if you have existing MAC OS system, you can create USB with original AppStore version of High Sierra with  Clover Bootloader. 

<b>WARNING ! ! ! - For bootable USB don't use USB 3.x versions.  If you will use USB 3.0 your  installation will be corupted in boot process. Support only for 2.x and  1.x versions of USB. Or you can looking for some guide to run installation from USB 3.0 on your T430.</b>

<hr>

<b>2. step - Installation MAC OS</b> - Boot installation from created USB stick, and format your SSD / HDD  as MAC OS Extended (Journaled)- [HSF] with scheme GUID Partition Map. 

<font color="red"><b><i>!!! You can use new format APFS if you have SSD (APFS was not tested for this T430 guide). !!!</i></b></font>

When is disk erased , close Disk utility window and click on Install macOS. Select disk where will be MAC installed and start            installation.  During installation will be your computer restarted and after next boot will be installed MAC OS to HDD/SSD. After        installation, boot macOS from USB stick. 


<hr>

<b>3. step - CLOVER INSTALLATION</b> - Recommended version of Clover is in Olarila USB stick in FILES folder) or download latest version of Clover EFI bootloader here >>> https://sourceforge.net/projects/cloverefiboot/  <<< and run installation of Clover. Select installation to HDD/SSD with system. 
Click on customize button  and select:  <b>Install for UEFI Booting Only and Install Clover in the ESP </b> and in Driver64UEFI select only <b>OsxAptioFix2Drv-64 or OsxAptioFix3Drv-64</b> 
<h4>WARRNING ! ! ! select only one version of OsxAptioFix, no more drivers ! ! !</h4>
After customization click on Install button. 
<hr>

<b>4. step - Patch your own DSDT</b> - This is really necessary step. You must generate own DSDT files, because our T430 models can be different in hardware and Bios settings and versions. 

Unplug your USB stick from laptop and restart your system. 
When will be displayed CLOVER Boot menu press <b>F4</b> on your keyboard, Clover will block mouse and keyboard for few seconds (3-15 sec.) and after few seconds again activate mouse and keyboard functions. Now plug-in USB stick with installator and reset laptop.
Now boot macOS from USB stick again. 




  
