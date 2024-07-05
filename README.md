# Release
## System and OS Requirements:<br>
1. Windows 10 and above
2. Minimum 2 cores
3. 2GB RAM
4. 30GB SSD
2. Java version 11 and above must be installed in your VPS. If your windows VPS doesn't have it, download it from [Here](https://www.java.com/en/download/) and set java in your windows environment.
## Installing and configuring a Blockchain Natzionale Sarda BNS full node for mining FFTs (Food Forest Token) on a Windows PC/VPS<br>
 Step 1: Click Here and [Download](https://github.com/Food-Forest-Sardegna/release/releases/download/v1.3.6-v1.5.3/fft-all-1.5.3.jar) the jar file.<br>
 Step 2: Download and unzip [this folder](https://github.com/Food-Forest-Sardegna/release/archive/refs/heads/main.zip)<br>
 Step 3: Place the fft-all-1.5.3.jar inside the folder mentioned in step 2.<br>
 Step 4: Modify the configuration file to activate your node in **mainnet.conf**<br>
 Step 5: Click the file inside the folder named as **"start.bat"**

## How to run a BNS Node with Windows OS
**Step 1:** Download the [BNS Desktop Wallet](https://github.com/Food-Forest-Sardegna/FFTfx-Wallet/archive/refs/heads/main.zip) on yours Windows PC. Open the Desktop Wallet of the BNS, and create a new account inside the **Mainnet chain**<br> 
**Step 2:** Notedown/copy the Encoded Seed of your account from the BNS wallet settings area. (This Seed will be used within the edits to be done inside the mainnet.conf file, to run the node)<br>
**Step 3:** Open the mainnet.conf file in any text editor. (Text Note, NotePad etc)<br>
**Step 4:** Edit the mainnet.conf file accordingly, in the lines showed below, and save it<br>
a) node-name = "Type Your Node Name Here"<br> (Line 78 of the mainnet.conf file)
b) declared-address = "127.0.0.1:6860" #declared ip address of your node<br> (Line 79 of the mainnet.conf file)
c) seed = "Enter_Your_Encoded_Backup_Seed_Here_From_The_BNS_Wallet" <br> (Line 89 of the mainnet.conf file)
d) password = "Enter any Random Password Here to protect your wallet" #Enter a 15 minimum characters strong password to protect your Wallet<br> (Line 90 of the mainnet.conf file)
e) save the mainnet.conf file after making the changes needed indicated above<br>
f) run the file start.bat by double clicking it, and the node should start downloading the blocks to get in synch with the Blockchain Natzionale Sarda BNS.<br>

If an error occurs while the node is starting up, it means that some error has been made in the mainnet.conf file edits.

If no errors occur, congratulations, you are now officially operating a node inside the BNS, and your node will appear inside the dedicated section of the connected peers inside the BNS Explorer area.

## Installing and configuring a Blockchain Natzionale Sarda BNS full node for mining FFTs (Food Forest Token) on a Linux PC/Server
## System and OS Requirements:<br>
1. Ubuntu 20 VPS in case of Linux<br>
2. Minimum 2 cores<br>
3. 2GB RAM<br>
4. 30GB SSD<br>

All commands are issued as root. If you do not use your root account most commands would probably require 'sudo' to work. Eg. "sudo apt update"<br>

## How to run a BNS node with Linux OS

**Step 1:** login into your Linux pc/server terminal with the root account<br>

**Step 2:** Type the command showed below<br>
>sudo apt update<br>
>sudo apt upgrade<br>
 
**Step 3:** Install the needed Java development kit, using the following commands<br>
> sudo apt install openjdk-11-jre <br>
> sudo apt install openjdk-11-jdk <br>
> sudo apt update <br>

Once the Java kit its installed, check if the version is the latest by using this command:
> java -version

## Linux Server Step
**Step 4:** Download the latest jar and mainnet.conf file.<br>
Enter the following commands one by one inside your linux server/pc to download both files accordingly<br>
> sudo wget https://github.com/Food-Forest-Sardegna/release/releases/download/v1.3.6-v1.5.3/fft-all-1.5.3.jar<br>
> sudo wget https://raw.githubusercontent.com/Food-Forest-Sardegna/release/main/mainnet.conf<br>

## Windows PC Step
**Step 5:** Download the [BNS Desktop Wallet](https://github.com/Food-Forest-Sardegna/FFTfx-Wallet/archive/refs/heads/main.zip) on yours Windows PC.<br>
Open the Desktop Wallet of the BNS, and create a new account inside the **Mainnet chain**. Notedown/copy the Encoded Seed of your account from the BNS wallet settings area. (This Seed will be used within the edits to be done inside the mainnet.conf file, to run the node)
## Linux Server Step
Type the linux commands provided below, and press the “Enter” button after each of them, to be able to make the required changes inside the mainnet.conf file<br>
> screen<br>
> sudo vi mainnet.conf<br>

Once the file is opened, press the **Insert button** to edit the mainnet.conf file itself<br>

**Step 6:** Edit the mainnet.conf file accordingly, in the lines showed below, and save it<br>
a) node-name = "Type Your Node Name Here"<br> (Line 78 of the mainnet.conf file)
b) declared-address = "127.0.0.1:6860" #declared ip address of your node<br> (Line 79 of the mainnet.conf file)
c) seed = "Enter_Your_Encoded_Backup_Seed_Here_From_The_BNS_Wallet"<br> (Line 89 of the mainnet.conf file)
d) password = "Your Password Here" #Enter a 15 minimum characters strong password to protect your Wallet<br> (Line 90 of the mainnet.conf file)
e) use the commands below to save the changes inside the mainnet.conf file <br>

Press the Escape (**Esc**) button and type the below command 
>:w

Next press the **Enter** button.
Now type **:qa!** and press **Enter** to get back into the writing mode.

**Note**: if something went wrong during the editing or you don't wanna to save it, just press the "Esc" button and type **:qa!** to exit it by pressing the Enter button after. Use the command **sudo vi mainnet.conf** again to edit the file if necessary. Be assured that your server have the latest or the mentioned java version (see Step 3).

Now to start the node simply use the following command:
>java -jar fft-all-1.5.3.jar mainnet.conf

The node will start downloading and synching the Blockchain Natzionale Sarda BNS. If an error occurs while the node is starting up, it means that some error has been made in the mainnet.conf file edits. Use the “Note” indications to edit the file again.
If no errors occur, congratulations, you are now officially operating a node inside the BNS, and your node will appear inside the dedicated section of the connected peers inside the BNS Explorer area.
When all blocks are synched, you can detach the screen by pressing **CTRL+d** and close the window. The node has been set to run in the background processes of your Linux PC/VPS.


Congratulations on your choice, because it is thanks to free individuals like you that the BNS is decentralised and strong in its actions.
