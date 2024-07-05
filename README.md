# Release

## System and OS Requirements:<br>

1. Windows 10 and above
2. Minimum 2 cores
3. 2GB RAM
4. 30GB SSD
2. Java version 11 and above must be installed in your VPS. If your windows VPS doesn't have it, download it from [Here](https://www.java.com/en/download/) and set java in your windows environment.

## Installing and configuring a Blockchain Natzionale Sarda BNS full node for mining FFTs (Food Forest Token) on a Windows PC/VPS<br>

 Step 1: Download and unzip [the " Release Main" folder clicking here](https://github.com/Food-Forest-Sardegna/release/archive/refs/heads/main.zip)<br>

 Step 2: Now [click HERE and download](https://github.com/Food-Forest-Sardegna/release/releases/download/v1.3.6-v1.5.3/fft-all-1.5.3.jar) the newest .jar file of the nodes version.<br>

 Step 3: Place the fft-all-1.5.3.jar just downloaded inside the "Release Main" unzipped folder, mentioned in step 1, with the other files present in it, ReadMe.md - mainnet.conf and start.bat file.<br>

# Now you are ready to proceed with the next steps :

 Step 4: Download the [BNS Desktop Wallet](https://github.com/Food-Forest-Sardegna/BNS-Desktop-Wallet/archive/refs/heads/main.zip) on yours Windows PC. Open the Desktop Wallet of the BNS, and create a new account inside the **Mainnet chain**<br>

Step 5: Notedown/copy the Encoded Seed of your account from the BNS wallet settings area. (This Encodeed Seed will be used within the edits to be done inside the mainnet.conf file, to run the node).<br>

Step 6: Open the mainnet.conf file in any text editor. (Text Note, NotePad etc)<br>

Step 7: Edit the mainnet.conf file accordingly, in the lines showed below, and save it<br>

a) node-name = "Type Your Node Name Here"<br> (Line 78 of the mainnet.conf file)

b) declared-address = "127.0.0.1:6860" #declared ip address of your node<br> (Line 79 of the mainnet.conf file)

c) seed = "Enter_Your_Encoded_Backup_Seed_Here_From_The_BNS_Wallet" <br> (Line 89 of the mainnet.conf file)

d) password = "Enter a strong Password here to protect your wallet" #Enter a strong password that has 15 characters minimum to protect your Wallet<br> (Line 90 of the mainnet.conf file)

e) save the mainnet.conf file after making the changes needed indicated above<br>

Step 8: Run the file start.bat by double clicking it, and the node should start downloading the blocks to get in synch with the Blockchain Natzionale Sarda blocks forged till now.<br>

If an error occurs while the node is starting up, it means that some error has been made in the mainnet.conf file edits.

If no errors occur, congratulations, you are now officially operating a node inside the BNS, and your node will appear inside the dedicated section of the [connected peers inside the BNS Explorer area visible here](https://fftexplorer.com/peers).

## Installing and configuring a Blockchain Natzionale Sarda BNS full node for mining FFTs (Food Forest Token) on a Linux PC/Server

## System and OS Requirements:<br>

1. Ubuntu 20 VPS in case of Linux<br>
2. Minimum 2 cores<br>
3. 2GB RAM<br>
4. 30GB SSD<br>

PLEASE KEEP IN MIND! THE DESKTOP WALLET IS ONLY AVAILABLE FOR WINDOWS OS
## Windows PC Step
Download the [BNS Desktop Wallet](https://github.com/Food-Forest-Sardegna/BNS-Desktop-Wallet/archive/refs/heads/main.zip) on yours Windows PC.<br>
Open the Desktop Wallet of the BNS, and create a new account inside the **Mainnet chain**. Notedown/copy the Encoded Seed of your account from the BNS wallet settings area. (This Seed will be used within the edits to be done inside the mainnet.conf file, to run the node). 

If you dont have a Windows PC, but you want to start a node, you can be able to do so by using our [Web Wallet accessible by clicking here](https://portafolliu.blockchainnatzionalesarda.online/) to create a new account, and in order to obtain your Encoded Seed, you will have to click on the "Account Back Up" info, on the top right corner of the web wallet dashboard, click on the "COPY" button in the menu, and pasting the whole backup info inside a note text file or word document. You will find your encoded seed there, and will be possible to use it for your node set up.


## How to run a BNS node with Linux OS

All commands are issued as root. If you do not use your root account most commands would probably require 'sudo' to work. Eg. "sudo apt update"<br>

**Step 1:** Login into your Linux pc/server terminal with the root account<br>

**Step 2:** Type the command showed below<br>

>sudo apt update<br>

>sudo apt upgrade<br>
 
In case of updates/upgrades needing a confirmation, type "Y" when asked, and confirm with the Enter button of your keyboard.

**Step 3:** Install the needed Java development kit, using the following commands<br>

> sudo apt install openjdk-11-jre <br>

When finished use the next command
> sudo apt install openjdk-11-jdk <br>

When done completely, use the command
> sudo apt update <br>

Once the Java kit its installed, check if the version is the latest by using this command:
> java -version

## Now you are ready for the next step:

**Step 4:** Download the latest jar and mainnet.conf file as explained below.<br>

Enter the following commands one by one inside your linux server/pc to download both files accordingly<br>

> sudo wget https://github.com/Food-Forest-Sardegna/release/releases/download/v1.3.6-v1.5.3/fft-all-1.5.3.jar<br>

After the download is finished, use the next command below
> sudo wget https://raw.githubusercontent.com/Food-Forest-Sardegna/release/main/mainnet.conf<br>

**Step 5:**

Type the linux commands provided below, and press the “Enter” button after typing them, to be able to make the required changes inside the mainnet.conf file<br>

First command
> screen<br>

Second command
> sudo vi mainnet.conf<br>

Once the file is opened, press the **Insert button** (INS) to edit the mainnet.conf file itself<br>

**Step 6:** Edit the mainnet.conf file accordingly, in the lines showed below, and save it<br>

**Note**: if something goes wrong during the editing or you don't wanna to save the file with wrong edits, just press the "Esc" button and type **:qa!** to exit it by pressing the Enter button after. 
Use the command **sudo vi mainnet.conf** again to edit the file if necessary.

a) node-name = "Type Your Node Name Here"<br> (Line 78 of the mainnet.conf file)

b) declared-address = "127.0.0.1:6860" #declared ip address of your node<br> (Line 79 of the mainnet.conf file)

c) seed = "Enter_Your_Encoded_Backup_Seed_Here_From_The_BNS_Wallet"<br> (Line 89 of the mainnet.conf file)

d) password = "Your Password Here" #Enter a 15 minimum characters strong password to protect your Wallet<br> (Line 90 of the mainnet.conf file)

e) use the commands below to save the changes inside the mainnet.conf file <br>

Press the Escape (**Esc**) button and type the below command 

>:w

Next press the **Enter** button.

Now type **:qa!** and press **Enter** to get back into the writing mode.

**Step 7:** To start the node now, simply use the following command:

>java -jar fft-all-1.5.3.jar mainnet.conf

The node will start downloading and synching the Blockchain Natzionale Sarda Blocks forged till now. If an error occurs while the node is starting up, it means that some error has been made in the mainnet.conf file edits, and you have to use the “Step 6” indications to edit the file again.

If no errors occur, congratulations, you are now officially operating a node inside the BNS, and your node will appear inside the dedicated section of the [connected peers inside the BNS Explorer area visible here](https://fftexplorer.com/peers).

When all blocks are synched, you can detach the screen by pressing **CTRL+d** and close the window. The node has been set to run in the background processes of your Linux PC/VPS.


Congratulations on your choice, because it is thanks to free individuals like you that the BNS is decentralised and strong in its actions.
