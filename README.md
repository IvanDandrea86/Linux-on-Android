# Linux on Android


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





