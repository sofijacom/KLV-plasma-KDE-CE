# *KDE-plasma-Void-CE*

![Снимок экрана_20240710_134306](https://github.com/sofijacom/KDE-plasma-Void-CE/assets/107557749/33d847a9-8d59-43df-9db1-fff722148172)


![Снимок экрана_20240708_013723](https://github.com/sofijacom/KDE-plasma-Void-CE/assets/107557749/bf8b0f1a-d484-4b83-9caf-01968162fb11)


![2024-07-07_20-41](https://github.com/sofijacom/KDE-plasma-Void-CE/assets/107557749/f4306dcd-528f-4439-a9a4-38aa9a10f63d)

1) Create a folder `KDE-plasma-Void-CE` typing in the terminal `mkdir -p KDE-plasma-Void-CE`

2) Open a terminal in the created folder `KDE-plasma-Void-CE` or go to the folder by typing in the terminal

   - `cd KDE-plasma-Void-CE`

3) Place the build script  `FR_minimal_KDE_plasma_desktop.sh` in the created folder.
   
4) Make it executable.`chmod +x FR_minimal_KDE_plasma_desktop.sh`

5) Enter in terminal `./FR_minimal_KDE_plasma_desktop.sh`

6) Wait for the build to finish.

7) After the build is complete to package `07firstrib_rootfs` into `07KDE-plasma-Void-CE-x.x.sfs` where x.x is your build number.

8) Type in terminal.

```
mksquashfs 07firstrib_rootfs 07KDE-plasma-Void-CE-x.x.sfs -noappend -comp xz -b 512k
```
  - where x.x is your build number.

9) Delete the `07firstrib_rootfs` folder.


```
 git clone https://github.com/sofijacom/KDE-plasma-Void-CE.git
```
