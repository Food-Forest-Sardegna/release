# releases
## System and OS Requirements:<br>
1. Windows 10 and above
2. Minimum 2 cores
3. 2GB RAM
4. 30GB SSD
2. Java version 11 and above must be installed in your VPS. If your windows VPS doesn't have it download it from [Here](https://www.java.com/en/download/) and set java in your windows environment.
## Installing and configuring a FFS Blockchain full node for FFT mining on a Windows PC/VPS<br>
 Step 1: Click Here and [Download](https://github.com/Food-Forest-Sardegna/release/releases/download/v1.3.6-v1.5.3/fft-all-1.5.3.jar) the jar file.<br>
 Step 2: Modify the configuration file to activate your node in **mainnet.conf**<br>
 Step 3: Click the file inside the folder named as **"start.bat"**

## How to run Node the FFT Node
**Step 1:** Download the [FFT Desktop Wallet](https://github.com/Food-Forest-Sardegna/FFTfx-Wallet/archive/refs/heads/main.zip) and set mainnet inside the FFT wallet to generate a blank FFT account. (without funds)<br> 
**Step 2:** Notedown the Encoded seed from your FFT wallet account, looking inside the settings. (It will be required for the edits to be done inside the mainnet.conf file)<br>
**Step 3:** Open the mainnet.conf file in any text editor. (Text Note, NotePad etc)<br>
**Step 4:** Change the below lines in mainnet.conf and save it<br>
a) node-name = "Type Your Node Name Here"<br>
b) declared-address = "127.0.0.1:6860" #declared ip address of your node<br>
c) seed = "Enter_Your_Encoded_Backup_Seed_Here_From_FFT_Wallet" <br>
d) password = "Enter any Random Password Here to protect your wallet" #Enter the 15 words any Strong password to protect your Wallet<br>
e) save the mainnet.conf file after making above changes <br>
f) run the file start.bat by double clicking it and the node should start downloading the blocks to get in synch with the FFS Blockchain.<br>

If an error occurs while the node is starting up, it means that some error has been made in the mainnet.conf file

Good Luck and Prosperity with Food Forest Token Mining and Leasing.

## Installing and configuring a  FFS Blockchain full node for FFT mining on a Linux PC/Server
## System and OS Requirements:<br>
1. Ubuntu 20 VPS in case of Linux<br>
2. Minimum 2 cores<br>
3. 2GB RAM<br>
4. 30GB SSD<br>

All commands are issued as root. If you do not use your root account most commands would probably require 'sudo' to work. Eg. "sudo apt update"<br>

## How to run an FFT Node of the FFS Blockchain

**Step 1:** login into you Linux pc/server terminal with the root account<br>

**Step 2:** Type the command showed below<br>
>sudo apt update<br>
>sudo apt upgrade<br>
 
**Step 3:** Install the Java development kit using the following commands<br>
> sudo apt install openjdk-11-jre <br>
> sudo apt install openjdk-11-jdk <br>
> sudo apt update <br>

Once its installed check if the version is the latest.
> java -version

## Linux Server Step
**Step 4:** Download the latest jar and mainnet.conf file.<br>
Enter following command one by one in linux server to download both<br>
> sudo wget https://github.com/Food-Forest-Sardegna/release/releases/download/v1.3.6-v1.5.3/fft-all-1.5.3.jar<br>
> sudo wget https://raw.githubusercontent.com/Food-Forest-Sardegna/release/main/mainnet.conf<br>

## Windows PC Step
**Step 5:** Download the [FFT Desktop Wallet](https://github.com/Food-Forest-Sardegna/FFTfx-Wallet/archive/refs/heads/main.zip) on windows PC.<br>
Open Desktop Wallet, Create a new account inside the **Mainnet chain** copy and save your Encoded backup seed found inside the settings, this seed will be used inside mainnet.conf to run the node.

## Linux Server Step
Type the below linux commands, and press the “Enter” button after each of them, make the required changes in the mainnet.conf file<br>
> screen<br>
> sudo vi mainnet.conf<br>

Once file is opened, Press the **Insert button** to edit mainnet.conf<br>

**Step 6:** Change the below lines in mainnet.conf and save it<br>
a) node-name = "Type Your Node Name Here"<br>
b) declared-address = "127.0.0.1:6860" #declared ip address of your node<br>
c) seed = "Enter_Your_Encoded_Backup_Seed_Here_From_FFT_Wallet"<br>
d) password = "Your Password Here" #Enter the 15 words any Strong password to protect your Wallet<br>
e) use the commands below to save the changes inside the mainnet.conf file <br>

Press Escape (**Esc**) button and type the below command 
>:w

Next press the **Enter** button.
Now type **:qa!** and press **Enter** to get back into the writing mode.

**Note**: if something went wrong during the editing or you don't wanna to save it, just press Esc and type **:qa!** to exit by pressing the Enter button after. Use the command **sudo vi mainnet.conf** again to edit the file if necessary. Be ensure your server must have latest or mentioned java version as mentioned in Step 3.

Now to start the node simply use the following command:
>java -jar fft-all-1.5.3.jar mainnet.conf

The node will start downloading and synching the blockchain. If any error appears during the activation of the node means something has been inserted wrongly in the mainnet.conf file. Use the “Note” indications to edit the file again.

When all blocks are synched, then you can detach the screen by pressing **CTRL+d** and close the window. The node has been set to run in background process of your Linux PC/VPS.


## Updating node from old version to new version
### ⚠️Warning : **Be Ensure you notedown Encoded seed of your node which is available in Step 6 (c). Losing of that encoded seed means lead to loss of node funds.**  

Step1 : Enter into linux server

Step2 : Type following command, press enter to see and attach screen of running node
> screen -ls
 
it will show the list of running screen note down that number

Step 3: Type below command, press enter
> screen -r -d screennumber

Where screennumber = From Step 2

Step 4: Press ”ctrl+c” to stop the running node.

Step 5: Type the following command to delete the existing fft folder containing all nodes files. 
Warning: ⚠️ Be ensure before deleting this folder you have Encoded Seed of your node.  

> sudo rm -rf /opt/fft

Step6: Follow the steps from Here to install node(https://github.com/Food-Forest-Sardegna/release?tab=readme-ov-file#installing-and-configuring-a--ffs-blockchain-full-node-for-fft-mining-on-a-linux-pcserver)


Good Luck and Prosperity with the Mining and Leasing of Food Forest Token.