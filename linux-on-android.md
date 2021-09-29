# Linux on Android
#### [EN](linux-on-android.md#EN)/[FR](linux-on-android.md#FR)

---
### Here you will find a list of istruction to have a linux shell on your Android smartphone.
---
## Index<a name="EN"></a>

1. [About Termux](linux-on-android.md#About)
1. [Install Termux](linux-on-android.md#Install)
2. [Update the System](linux-on-android.md#Update)
3. [Install Ubuntu](linux-on-android.md#Ubuntu)
4. [Bonus / Running VSCODE](linux-on-android.md#VSCODE)
5. [Credits](linux-on-android.md#Credit)

---

## About Termux <a name="About"></a>
---
 Termux is an Android terminal emulator and Linux environment app that works directly with no rooting or setup required. A minimal base system is installed automatically - additional packages are available using the APT package manager.

## Install termux <a name="Install"></a>
---
You can download Termux on [GooglePlay](https://play.google.com/store/apps/details?id=com.termux) or [F-Droid](https://f-droid.org/packages/com.termux/)


## Update the System <a name="Update"></a>
---
After install Termux you must update the system and istall some packages.

### Update Termux
```  
apt-get update && apt-get upgrade -y
```
### Update wget/proot/git
```  
apt-get install wget -y
```
```  
apt-get install proot -y
```
```
apt-get install git -y
```

## Install Ubuntu <a name="Ubuntu"></a>
---
MFD Gaming has a script which will do the heavy lifting for this and install Ubuntu 20.10 (at time of writing) into Termux 



### Go to HOME Folder
```
cd ~
```

### Download script:
```
git clone https://github.com/MFDGaming/ubuntu-in-termux.git
```
### Go to script folder:
```
cd ubuntu-in-termux
```
### Give execution permission:
```
chmod +x ubuntu.sh
```
### Run the script:
```
./ubuntu.sh -y
```
### Now just start ubuntu:
```
./startubuntu.sh
```
Update Ubuntu
```
apt update 
```
apt upgrade
Install Wget
```
apt install wget
```
----

## Bonus Running VSCODE <a name="VSCODE"></a>
----
### Install VSCode on Termux

Now Ubuntu is running in Termux the next step is to install the ARM version of VS Code into the Termux environment

```
wget https://github.com/cdr/code-server/releases/download/v3.12.0/code-server-3.12.0-linux-amd64.tar.gz
```
### Extract the archive

```
tar -xvf ./code-server-3.12.0-linux-amd64.tar.gz
```
```
rm ./code-server-3.12.0-linux-amd64.tar.gz
```
```

cp -r ./code-server-3.12.0-linux-amd64/lib/
```
```
ln -s ./code-server-3.12.0-linux-amd64/code-server/bin/
```

### Run the Server

```
code-server
```
Copy the passcode it generates as you'll need this to login later

Alternative method for getting password
```
tail ~/.config/code-server/config.yaml
```
Open in Browser on Android Device
```
localhost:8080 
```
---

## Enjoy coding on you Smartphone!!!

---

## Credits <a name="Credit"></a>

* [Terminux Site](https://termux.com/)
* [GooglePlay Site](https://play.google.com/)
* [F-Droid Site](https://f-droid.org/)
* [MFDGaming/ubuntu-in-termux](https://github.com/MFDGaming/ubuntu-in-termux)
* [Davide Field Tech Blog Post](https://tech.davidfield.co.uk/running-vs-code-on-an-android-device/)

---
## Index<a name="FR"></a>

1. [À propos de Termux](linux-on-android.md#AboutFr)
2. [Installer Termux](linux-on-android.md#InstallFr)
3. [Mettre à jour le système](linux-on-android.md#UpdateFr)
4. [Install Ubuntu](linux-on-android.md#UbuntuFr)
5. [Bonus / Exécuter VSCODE](linux-on-android.md#VSCODEFr)
6. [Credits](linux-on-android.md#CreditFr)

---

## À propos de Termux <a name="AboutFr"></a>
---
Termux est un émulateur de terminal Android et une application d'environnement Linux qui fonctionne directement sans avoir besoin d'être rooté ou configuré. Un système de base minimal est installé automatiquement - des paquets supplémentaires sont disponibles en utilisant le gestionnaire de paquets APT.

## Installer termux <a name="InstallFr"></a>
---
Vous pouvez télécharger Termux sur [GooglePlay](https://play.google.com/store/apps/details?id=com.termux) ou[F-Droid](https://f-droid.org/packages/com.termux/)


## Mettre à jour le système <a name="UpdateFr"></a>
---
After install Termux you must update the system and istall some packages.

### Mise à jourTermux
```  
apt-get update && apt-get upgrade -y
```
### Mise à jour wget/proot/git
```  
apt-get install wget -y
```
```  
apt-get install proot -y
```
```
apt-get install git -y
```

## Installer Ubuntu <a name="UbuntuFr"></a>
---
MFD Gaming a un script qui fera le gros du travail et installera Ubuntu 20.10 (au moment de l'écriture) dans Termux


### Aller au dossier HOME
```
cd ~
```

### Télécharger script:
```
git clone https://github.com/MFDGaming/ubuntu-in-termux.git
```
### Aller au dossier script:
```
cd ubuntu-in-termux
```
### Donner l'autorisation d'exécution:
```
chmod +x ubuntu.sh
```
### Exécuter le script:
```
./ubuntu.sh -y
```
### Maintenant, il suffit de commencer ubunut:
```
./startubuntu.sh
```
Update Ubuntu
```
apt update 
```
apt upgrade
Install Wget
```
apt install wget
```
----

## Bonus Exécuter VSCODE <a name="VSCODEFr"></a>
----
### Installer VSCode sur Termux

Maintenant qu'Ubuntu tourne dans Termux, la prochaine étape consiste à installer la version ARM de VS Code dans l'environnement Termux.

```
wget https://github.com/cdr/code-server/releases/download/v3.12.0/code-server-3.12.0-linux-amd64.tar.gz
```
### Extraire l'archive

```
tar -xvf ./code-server-3.12.0-linux-amd64.tar.gz
```
```
rm ./code-server-3.12.0-linux-amd64.tar.gz
```
```

cp -r ./code-server-3.12.0-linux-amd64/lib/
```
```
ln -s ./code-server-3.12.0-linux-amd64/code-server/bin/
```

### Exécuter le serveur

```
code-server
```
Copiez le code d'accès qu'il génère car vous en aurez besoin pour vous connecter ultérieurement.

Méthode alternative pour obtenir le mot de passe
```
tail ~/.config/code-server/config.yaml
```
Ouvrir dans le navigateur sur un appareil Android
```
localhost:8080 
```
---
## Amusez-vous à coder sur votre Smartphone !!

---

## Credits <a name="Credit"></a>

* [Terminux Site](https://termux.com/)
* [GooglePlay Site](https://play.google.com/)
* [F-Droid Site](https://f-droid.org/)
* [MFDGaming/ubuntu-in-termux](https://github.com/MFDGaming/ubuntu-in-termux)
* [Davide Field Tech Blog Post](https://tech.davidfield.co.uk/running-vs-code-on-an-android-device/)




