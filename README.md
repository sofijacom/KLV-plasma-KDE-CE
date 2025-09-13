<div align="center">
   
# *KLV-plasma-KDE-CE*


<div align="center">
<img width="750" height="458" alt="laptop" src="https://github.com/user-attachments/assets/7e1637d3-755f-4a07-ba67-27a2cc03e8f1" />


<a id="installation"></a>  
<img src="https://github.com/user-attachments/assets/7e1e2fa0-ab50-4901-a024-fe731fb44ab3" width="200"/>
---

1) Create a folder `KLV-plasma-KDE-CE` typing in the terminal `mkdir -p KLV-plasma-KDE-CE`

2) Open a terminal in the created folder `KLV-plasma-KDE-CE` or go to the folder by typing in the terminal

   - `cd KLV-plasma-KDE-CE`

3) Place the build script  `FR_minimal_KDE_plasma_desktop.sh` in the created folder.
   
4) Make it executable.`chmod +x FR_minimal_KDE_plasma_desktop.sh`

5) Enter in terminal `./FR_minimal_KDE_plasma_desktop.sh`

6) Wait for the build to finish.

7) After the build is complete to package `07firstrib_rootfs` into `07KLV-plasma-KDE-x.x.sfs` where x.x is your build number.

8) Type in terminal.

```
mksquashfs 07firstrib_rootfs 07KLV-plasma-KDE-x.x.sfs -noappend -comp xz -b 512k
```
  - where x.x is your build number.

9) Delete the `07firstrib_rootfs` folder.


```
 git clone https://github.com/sofijacom/KLV-plasma-KDE-CE.git
```
