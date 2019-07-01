# My often used Terminal Cmd´s WIP
I will add them as I use them.

## Loop Mount a EXT4 .img
# Tools
* simg2img
If its already installed and in your path thats fine if not
place it in your working folder and ensure its got the correct
permissions.
# Method
So you have a ext4 system.img and you wish to view the contents.
First make a folder named ¨working¨ then inside that a folder called ¨mounted¨
Place the ext4.img & simg2img in the folder called ¨working¨.
Now open the Terminal in working or cd to it.

```cd ~/working```

## Uncompress the EXT4

The following cmd will decompress the ext4 to a raw image.

```simg2img system.img system.img.raw```

## Mount it to our folder called mounted.

```sudo mount -t ext4 -o loop system.img.raw ~/working/mounted/```

# Github Stuff
## Add Kernel Source to github as example
## Method
Create a New Repository using your github home page.
EG: android_kernel_nokia_3.1
Now on your PC cd into the kernel-3.x folder and type the following.

```git init```
Then type this add all cmd (Why they dont tell you this on github I have no idea)

```git add --all```
This does what it says and adds all the files and folders in the kernel-3.x folder for uploading
After this follow githubs instructions.

```git commit -m "first commit"```

```git remote add origin git@github.com:bigrammy/android_kernel_nokia_3.1.git
```
Then finally push it to github
```git push -u origin master```

# Done

  



  






