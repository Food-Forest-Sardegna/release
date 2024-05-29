# PDF Document About Release how to install and run FFT Node 

[README - ITA.pdf](https://github.com/Food-Forest-Sardegna/release/files/7718831/README.-.ITA.pdf)

[README - ENG.pdf](https://github.com/Food-Forest-Sardegna/release/files/7718832/README.-.ENG.pdf)


# releases
## System and OS Requirements:<br>
1. Windows 10 and above
2. Minimum 2 cores
3. 2GB RAM
4. 30GB SSD
2. Java version 11 and above must be installed in your VPS. If your windows VPS doesn't have it download it from [Here](https://www.java.com/en/download/) and set java in your windows environment.
## Installing and configuring a FFS Blockchain full node for FFT mining on a Windows PC/VPS<br>
 Step 1: Click Here and [Download](https://github.com/Food-Forest-Sardegna/release/archive/refs/heads/main.zip) the Zip Folder and Unzip it.<br>
 Step 2: Modify the configuration file to activate your node in **mainnet.conf**<br>
 Step 3: Click the file inside the folder named as **"start.bat"**

## How to run Node the FFT Node
**Step 1:** Download the [FFT Desktop Wallet](https://github.com/Food-Forest-Sardegna/FFTfx-Wallet/archive/refs/heads/main.zip) and set mainnet inside the FFT wallet to generate a blank FFT account. (without funds) 
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
1. Ubuntu 18 VPS in case of Linux<br>
2. Minimum 2 cores<br>
3. 2GB RAM<br>
4. 30GB SSD<br>

All commands are issued as root. If you do not use your root account most commands would probably require 'sudo' to work. Eg. "sudo apt update"<br>

## How to run an FFT Node of the FFS Blockchain

**Step 1:** login into you Linux pc/server terminal with the root account<br>

**Step 2:** Type the command showed below<br>
>apt update<br>
 
**Step 3:** Install the Java development kit using the following commands<br>
> sudo apt install openjdk-11-jre <br>
> sudo apt install openjdk-11-jdk <br>
> sudo apt update <br>

Once its installed check if the version is the latest.
> java -version

**Step 4:** Download the latest fullnode from Food-Forest-Sardegna repository.<br>
Link: [Latest Release](https://github.com/Food-Forest-Sardegna/release/archive/refs/heads/main.zip)

Command to download it on your Linux PC/Server<br>
> sudo wget https://github.com/Food-Forest-Sardegna/release/archive/refs/heads/main.zip<br>

**Step 5:** Download the [FFT Desktop Wallet](https://github.com/Food-Forest-Sardegna/FFTfx-Wallet/archive/refs/heads/main.zip) in Linux pc, create a new account inside the Mainnet chain and save your Encoded backup seed found inside the settings, to use it inside mainnet.conf when needed.

Type the commands below, and press the “Enter” button after each of them, to install Unzip in your Linux pc/server and being able next to make the required changes in the mainnet.conf file<br>
> sudo apt-get install unzip<br>
> unzip main.zip<br>
> cd release-main<br>
> screen<br>
> sudo vi mainnet.conf<br>

Press the **Enter button** to enable the ability to type and edit the file with vi editor<br>

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

**Note**: if something went wrong during the editing or you don't wanna to save it, just press Esc and type **:qa!** to exit by pressing the Enter button after. Use the command **sudo vi mainnet.conf** again to edit the file if necessary.

Now to start the node simply use the following command:
>java -jar fft-all-1.3.6.jar mainnet.conf

The node will start downloading and synching the blockchain. If any error appears during the activation of the node means something has been inserted wrongly in the mainnet.conf file. Use the “Note” indications to edit the file again.

When all blocks are synched, then you can detach the screen by pressing **CTRL+d** and close the window. The node has been set to run in background process of your Linux PC/VPS.

Good Luck and Prosperity with the Mining and Leasing of Food Forest Token.
