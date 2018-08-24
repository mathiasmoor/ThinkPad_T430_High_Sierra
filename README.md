# ThinkPad_T430_High_Sierra
<i>Guide to run MAC OS X - High Sierra on Lenovo ThinkPad T430 laptop

Vanilla MAC OSX - High Sierra almost perfect on Lenovo T430.</i>
<br><br>

<code>Sources: ThiagoSchetini and RehabMan.</code>


<h1>Step by Step - GUIDE</h1>

<b>1. step - Create Bootable USB with High Sierra installator.</b> I think, the best choice for  creating USB installator is Olarila image from this links: https://drive.google.com/file/d/1XIeW2LCRZPSNq3_RiTvefAGIT_2fGfaW/view?usp=sharing
or if you have existing MAC OS system, you can create USB with original AppStore version of High Sierra with latest version of Clover EFI. 

<hr>

<b>2. step - Installation MAC OS</b> - Boot installation from created USB stick, and format your SSD / HDD  as MAC OS Extended (Journaled)- [HSF] with scheme GUID Partition Map. 

<font color="red"><b><i>!!! You can use new format APFS if you have SSD (APFS was not tested for this T430 guide). !!!</i></b></font>

When is disk erased , close Disk utility window and click on Install macOS. Select disk where will be MAC installed and start            installation.  During installation will be your computer restarted and after next boot will be installed MAC OS to HDD/SSD. After          installation boot MAC OS with USB stick. 


<hr>

<b>3. step - download latest version of Clover EFI bootloader</b> here >>> https://sourceforge.net/projects/cloverefiboot/  <<< and run installation of Clover. Select installation to HDD/SSD with system. 
Click on customize and select:  <b>Install for UEFI Booting Only and Install Clover in the ESP </b> and in Driver64UEFI select only <b>OsxAptioFix2Drv-64 or OsxAptioFix3Drv-64</b> 
<h4>WARRNING ! ! ! select only one version of OsxAptioFix, no more drivers ! ! !</h4>
After customization click on Install button. 
<hr>

          
