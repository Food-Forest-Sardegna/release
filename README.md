English and Italian instructions on how to install a BNS node.
Istruzioni in Inglese e Italiano su come installare un nodo della BNS.

# Release ENGLISH

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

Step 7: Edit the mainnet.conf file accordingly, in the lines showed below, and save it.<br>

a) node-name = "Type Your Node Name Here"<br> (Line 78 of the mainnet.conf file)

b) declared-address = "127.0.0.1:6860" #declared ip address of your node<br> (Line 79 of the mainnet.conf file)

c) seed = "Enter_Your_Encoded_Backup_Seed_Here_From_The_BNS_Wallet" <br> (Line 89 of the mainnet.conf file)

d) password = "Enter a strong Password here to protect your wallet" #Enter a strong password that has 15 characters minimum to protect your Wallet<br> (Line 90 of the mainnet.conf file)

e) save the mainnet.conf file after making the changes needed indicated above<br>

Step 8: Run the file start.bat by double clicking it, and the node should start downloading the blocks to get in synch with the Blockchain Natzionale Sarda blocks forged till now.<br>

If an error occurs while the node is starting up, it means that some error has been made in the mainnet.conf file edits.

If no errors occur, congratulations, you are now officially operating a node inside the BNS, and your node will appear inside the dedicated section of the [connected peers inside the BNS Explorer area visible here](https://fftexplorer.com/peers).

Congratulations on your choice, because it is thanks to free individuals like you that the BNS is decentralised and strong in its actions.

§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§

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

If you dont have a Windows PC, but you want to start a node, you can be able to do so by using our [Web Wallet accessible by clicking here](https://portafolliu.blockchainnatzionalesarda.online/) to create a new account, and in order to obtain your Encoded Seed, you will have to click on the "Account Back Up" second icon found on the top right corner of the web wallet dashboard, than click on the "COPY" button in the menu appeard, and paste the whole backup info inside a note text file or word document. You will find your encoded seed there, and will be possible to use it for your node set up.

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

**Step 5:** Type the linux commands provided below, and press the “Enter” button after typing them, to be able to make the required changes inside the mainnet.conf file<br>

First command
> screen<br>

Second command
> sudo vi mainnet.conf<br>

Once the file is opened, press the **Insert button** (INS) to edit the mainnet.conf file itself<br>

**Note**: if something goes wrong during the editing or you don't wanna to save the file with wrong edits, just press the "Esc" button and type **:qa!** to exit it by pressing the Enter button after. 
Use the command **sudo vi mainnet.conf** again to edit the file from the beginning and its default form if necessary.

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

**Step 7:** To start the node now, simply use the following command:

>java -jar fft-all-1.5.3.jar mainnet.conf

Press the Enter button and the node will start downloading and synching the Blockchain Natzionale Sarda Blocks forged till now. If an error occurs while the node is starting up, it means that some error has been made in the mainnet.conf file edits, and you have to use the “Step 6” indications to edit the file again.

If no errors occur, congratulations, you are now officially operating a node inside the BNS, and your node will appear inside the dedicated section of the [connected peers inside the BNS Explorer area visible here](https://fftexplorer.com/peers).

When all blocks are synched, you can detach the screen by pressing **CTRL+d** and close the window. The node has been set to run in the background processes of your Linux PC/VPS.

Congratulations on your choice, because it is thanks to free individuals like you that the BNS is decentralised and strong in its actions.

---------------------------------------------------------------------------------------------------------------------------

# Rilascio ITALIANO

## Requisiti di sistema e del Sistema Operativo:<br>

1. Windows 10 o superiore
2. Minimo 2 core
3. 2GB RAM
4. 30GB SSD
2. La versione 11 o superiore di Java deve essere installata nel VPS. Se il vostro VPS Windows non ce l'ha, scaricatelo da [Qui](https://www.java.com/en/download/) e impostate Java nel vostro ambiente Windows.

## Installazione e configurazione di un nodo BNS della Blockchain Nazionale Sarda per il minaggio di FFT (Food Forest Token) su PC/VPS Windows<br>

 Passo 1: Scarica e decomprimi [la cartella "Release Main" cliccando qui](https://github.com/Food-Forest-Sardegna/release/archive/refs/heads/main.zip)<br>

 Passo 2: Ora [clicca QUI e scarica](https://github.com/Food-Forest-Sardegna/release/releases/download/v1.3.6-v1.5.3/fft-all-1.5.3.jar) il file .jar più recente della versione dei nodi.<br>

 Passo 3: Inserisci il file fft-all-1.5.3.jar appena scaricato all'interno della cartella decompressa "Release Main", menzionata al passo 1, mettendolo con gli altri file presenti al suo interno, ReadMe.md - mainnet.conf e il file start.bat .<br>

# Ora si è pronti per procedere con i passaggi successivi:

Passaggio 4: Scarica il [Portafoglio desktop BNS](https://github.com/Food-Forest-Sardegna/BNS-Desktop-Wallet/archive/refs/heads/main.zip) sul tuo PC Windows. Apri il Portafoglio Desktop della BNS e crea un nuovo account all'interno del **Mainnet**<br>

Passaggio 5: Annota/copia il seme codificato del tuo account che trovi nell'area delle impostazioni del portafoglio della BNS con l'incona ad ingranaggio. (Questo Seed codificato verrà utilizzato all'interno delle modifiche da apportare nel file mainnet.conf, per eseguire il nodo).<br>

Passaggio 6: Apri il file mainnet.conf in qualsiasi editor di testo. (Nota di testo, Blocco note ecc.)<br>

Passaggio 7: Modifica il file mainnet.conf ove necessario, nelle righe mostrate di seguito, e salvalo.<br>

a) node-name = "Digita qui il nome del tuo nodo/Type Your Node Name Here"<br> (Riga 78 del file mainnet.conf)

b) declared-address = "127.0.0.1:6860" #indirizzo IP dichiarato del tuo nodo(può rimanere invariato)<br> (Riga 79 del file mainnet.conf)

c) seed = "Inserisci qui il tuo Seed Codificato ottenuto nel portafoglio BNS/Enter_Your_Encoded_Backup_Seed_Here_From_The_BNS_Wallet" <br> (Riga 89 del file mainnet.conf)

d) password = "Inserisci qui una password complessa per proteggere il tuo portafoglio" #Inserisci una password complessa che contenga almeno 15 caratteri per proteggere il tuo portafoglio<br> (Riga 90 del file mainnet.conf)

e) salva il file mainnet.conf dopo aver apportato le modifiche necessarie indicate sopra<br>

Passo 8: Esegui il file start.bat facendo doppio clic su di esso e il nodo dovrebbe iniziare a scaricare i blocchi per entrare in sincronia con i blocchi forgiati fino ad ora nella Blockchain Nazionale Sarda .<br>

Se si verifica un errore durante l'avvio del nodo, significa che è stato commesso qualche errore nelle modifiche del file mainnet.conf.

Se non si verificano errori, congratulazioni, ora stai ufficialmente gestendo un nodo all'interno della BNS e il tuo nodo apparirà nella sezione dedicata dei [nodi connessi all'interno dell'Exploratore della BNS nell'area visibile qui](https://fftexplorer.com/peers ).

Complimenti per la tua scelta, perché è grazie a individui liberi come te che la BNS è decentralizzata e forte nelle sue azioni.

§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§§

## Installazione e configurazione di un nodo BNS della Blockchain Nazionale Sarda per il minaggio di FFT (Food Forest Token) su PC/Server Linux

## Requisiti di sistema e Sistema Operativo:<br>

1. Ubuntu 20 VPS in caso di Linux<br>
2. Minimo 2 core<br>
3. 2 GB di RAM<br>
4. SSD da 30 GB<br>

PER FAVORE RICORDA! IL PORTAFOGLIO DESKTOP È DISPONIBILE SOLO PER IL SISTEMA OPERATIVO WINDOWS

## Passaggio in PC Windows

Scarica il [Portafoglio Desktop della BNS](https://github.com/Food-Forest-Sardegna/BNS-Desktop-Wallet/archive/refs/heads/main.zip) sul tuo PC Windows.<br>
Apri il Portafoglio Desktop della BNS e crea un nuovo account all'interno del **Mainnet**. Annota/copia il seme codificato del tuo account che trovi nell'area delle impostazioni del portafoglio della BNS con l'incona ad ingranaggio. (Questo Seed codificato verrà utilizzato all'interno delle modifiche da apportare nel file mainnet.conf, per eseguire il nodo).

Se non hai un PC Windows, ma vuoi avviare un nodo, puoi farlo utilizzando il nostro [Portafoglio Web accessibile cliccando qui](https://portafolliu.blockchainnazionalesarda.online/) e creare qui un nuovo account. Per ottenere il tuo Seme Codificato quindi, dovrai fare clic sulla seconda icona che si trova nell'angolo in alto a destra della dashboard del portafoglio web, ovvero "Backup Account", contenente le informazioni del tuo conto appena creato, dovrai poi fare clic sul pulsante "COPIA" nel menu a tendina che viene mostrato, ed infine incollare tutte le informazioni di backup ottenute all'interno di un file di testo, nel blocco note ad esempio o in un documento Word. Ora vedrai il tuo seme codificato e sarà possibile utilizzarlo per la configurazione del tuo nodo.

## Come attivare un nodo BNS con sistema operativo Linux

Tutti i comandi vengono eseguiti come root. Se non usi il tuo account root, la maggior parte dei comandi probabilmente richiederanno "sudo" per funzionare. Per esempio. "sudo apt update"<br>

**Passaggio 1:** Accedi al terminale del tuo PC/server Linux con l'account root<br>

**Passaggio 2:** Digita il comando mostrato qui sotto<br>

>sudo apt update<br>

>sudo apt upgrade<br>

In caso di aggiornamenti/upgrade che necessitano di conferma, digitare "Y" quando richiesto e confermare con il pulsante Invio della tastiera.

**Passaggio 3:** Installa il kit di sviluppo Java necessario utilizzando i seguenti comandi<br>

> sudo apt install openjdk-11-jre <br>

Al termine utilizzare il comando successivo
> sudo apt install openjdk-11-jdk <br>

Alla fine dell'installazione, utilizzare il comando
>sudo apt upgrade<br>

Una volta installato il kit Java, verificare se la versione è l'ultima utilizzando questo comando:
> java -version

## Ora si è pronti per il passaggio successivo:

**Passaggio 4:** Scarica gli ultimi file jar e mainnet.conf come spiegato di seguito.<br>

Inserisci i seguenti comandi uno per uno nel tuo server/pc Linux per scaricare entrambi i file correttamente<br>

> sudo wget https://github.com/Food-Forest-Sardegna/release/releases/download/v1.3.6-v1.5.3/fft-all-1.5.3.jar<br>

Al termine del download, utilizzare il comando successivo indicato qui sotto
> sudo wget https://raw.githubusercontent.com/Food-Forest-Sardegna/release/main/mainnet.conf<br>

**Passaggio 5** Digita i comandi Linux forniti qui di seguito, premendo il pulsante "Invio" dopo aver digitato ciascun comando, per poter apportare le modifiche richieste all'interno del file mainnet.conf<br>

Primo comando
> screen<br>

Secondo comando
> sudo vi mainnet.conf<br>

Una volta aperto il file, premi il pulsante **Inserisci** (INS) per modificare il file mainnet.conf stesso<br>

**Nota**: se qualcosa va storto durante la modifica o non vuoi salvare il file con modifiche errate, premi semplicemente il pulsante "Esc" e digita **:qa!** per uscire e premendo poi il tasto Invio.
Se necessario, utilizza nuovamente il comando **sudo vi mainnet.conf** per modificare il file dall'inizio dalla sua forma predefinita.

**Passaggio 6:** Modifica il file mainnet.conf come necessario, nelle righe indicate qui di seguito, e salvalo<br>

a) node-name = "Digita qui il nome del tuo nodo/Type Your Node Name Here"<br> (Riga 78 del file mainnet.conf)

b) declared-address = "127.0.0.1:6860" #indirizzo IP dichiarato del tuo nodo(può rimanere invariato)<br> (Riga 79 del file mainnet.conf)

c) seed = "Inserisci qui il tuo Seed Codificato ottenuto nel portafoglio BNS/Enter_Your_Encoded_Backup_Seed_Here_From_The_BNS_Wallet" <br> (Riga 89 del file mainnet.conf)

d) password = "Inserisci qui una password complessa per proteggere il tuo portafoglio" #Inserisci una password complessa che contenga almeno 15 caratteri per proteggere il tuo portafoglio<br> (Riga 90 del file mainnet.conf)

e) utilizza le indicazioni e i comandi seguenti per salvare le modifiche all'interno del file mainnet.conf <br>

Premi il pulsante Escape (**Esc**) e digita il comando seguente

>:w

Quindi premi il pulsante **Invio**.

Ora digita **:qa!** e premi **Invio** per tornare alla modalità di scrittura.

**Passaggio 8:** Per avviare subito il nodo, utilizza semplicemente il seguente comando:

>java -jar fft-all-1.5.3.jar mainnet.conf

Premi il tasto INVIO e il nodo inizierà a scaricare e sincronizzare i blocchi forgiati fino ad ora della Blockchain Natzionale Sarda. Se si verifica un errore durante l'avvio del nodo, significa che è stato commesso qualche errore nelle modifiche del file mainnet.conf, e devi utilizzare le indicazioni del "Passaggio 6" per modificare nuovamente il file.

Se non si verificano errori, congratulazioni, ora stai ufficialmente gestendo un nodo all'interno della BNS e il tuo nodo apparirà nella sezione dedicata dei [nodi connessi all'interno dell'Exploratore della BNS nell'area visibile qui](https://fftexplorer.com/peers ).

Una volta sincronizzati tutti i blocchi, puoi staccare lo schermo premendo **CTRL+d** e chiudere la finestra. Il nodo è stato impostato per essere eseguito nei processi in background del tuo PC/VPS Linux.

Complimenti per la tua scelta, perché è grazie a individui liberi come te che la BNS è decentralizzata e forte nelle sue azioni.

-----------------------------------------------------------------------------------------------------------------------------------
