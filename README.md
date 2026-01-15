<div align="center">
   
# *KLV-plasma-KDE-CE*

  kio-admin
![Снимок экрана_20240708_125022](https://github.com/sofijacom/KDE-plasma-Void-CE/assets/107557749/a673415c-0856-40d9-85e6-c07322c60aa3)
=======

<img width="1366" height="833" alt="laptop" src="https://github.com/user-attachments/assets/fa0deedc-dc87-47a6-80ba-8c21ef8c140c" />


<a id="installation"></a>  
<img src="https://github.com/user-attachments/assets/7e1e2fa0-ab50-4901-a024-fe731fb44ab3" width="200"/>
---

<div align="left">
   
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
