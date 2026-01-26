<p align="center"><img src="/img/smalllogo.png" alt="validebagos logo" width="150"></p>

<h1 align="center">Validebag Os 0.4 Alpha Version</h1>

<p align="center">Validebag-OS is a lightweight Linux distribution currently in alpha, designed specifically for students.
 It is built from scratch to run efficiently on low-resource hardware and offers Turkish language support. 
 This early version invites testing and feedback from its users.
 https://www.reddit.com/r/ValidebagOsCommunity/</p>

<hr>

## How to install Validebag-Os on your computer or VM?


1. Before installing the os onto your machine, you need to have a empty partition. It needs to have at least 25 GB storage. When you make sure you have, you can go on with the installation process.

   - **At first, you need to create a mounting point on your hostsytem. You can create it with this command:**:
     ```
     mkdir /mnt/validebagos
     ```

2. After creating the directory, you need to create a varibale to simplify the installation guide.
   - **You can create the variable with this command:**:
     ```
     export validebagos=/mnt/validebagos
     ```

3. After creating the variable, you need to set umask in case your distro uses a different one.
   - **You can set umask with this command:**:
     ```
     umask 022
     ```


#Note: After each time you close or open a new terminal, you might need to set the umask and variable again. For making sure it is set correctly use this command:
   - **You can set check the variable and umask with this command:**:
     ```
     echo $validebagos
     umask
     ```

4. After checking the variable, you now need to mount your disk into the mountpoint.
   - **Use this command to make your variable a mountpoint:**:
     ```
     mkdir -pv $validebagos
     ```	
   - **After creating the mountpoint, use this command to mount your disk:**:
     ```
     mount -v -t ext4 /dev/sda(yourdisknumber) $validebagos
     `` 

5. After that, you need to be root user to continue. When you become root user, make sure to change the ownership of validebag os folder to root user.
 - **You can change the ownership with this command:**:
     ```
     chown -R root:root $validebagos
     case $(uname -m) in
     x86_64) chown -R root:root $validebagos/lib64 ;;
     esac
     ```






