## Docsify Setup

**Requirement of docsify**

- Distributor ID: Ubuntu <br>
- Description: Ubuntu 22.04.3 LTS <br>
- Release: 22.04 <br>
- Codename: jammy <br>

## Requirement Tools


**Node.js**<br>
**NPM**<br>

## Node.js ##

Node.js isn't directly used by Docsify, but it can be helpful when you're creating Docsify documentation. It helps you preview and test your documentation on your computer.<br>

 >Download Node.js
```bash
sudo apt install Node.js
```
>Check Node.js version <br>
```bash
sudo node -v
```
>Output <br>
```bash
v12.22.9
```
## NPM ##
Npm (Node Package Manager) is used Install and manage Docsify and its CLI globally.
>Download NPM
```bash
sudo apt install npm
```
>Check NPM version
```bash
sudo npm -v
```
>Output 
```bash
8.5.1
```

## Introduction Of Docsify
Docsify is a tool that helps you easily make documentation websites using simple text (Markdown). It makes your documentation look nice, with features like easy navigation, search, and different themes. To use it, you install Docsify on your computer and follow a few quick steps to set up your documentation.

## Installation and setup of Docsify

>Install Docsify CLI
```bash
npm install -g docsify-cli
```
>Check  docsify version
```bash
sudo docsify -v
```
>Output
```bash
docsify-cli version:
4.4.4
```
>Create a Documentation Directory
```bash
sudo mkdir Docsify
```
>Change Directory
```bash
cd /home/sanjit/Desktop/Docsify
```
>Output
```bash
sanjit@sanjit:~/Desktop/Docsify$ 
```
>Initialize the documentation directory with an empty index.html & README.md & doc.txt file
```bash
touch /home/sanjit/Desktop/Docsify/index.html
```

```bash
touch /home/sanjit/Desktop/Docsify/README.md
```

```bash
touch /home/sanjit/Desktop/Docsify/doc.txt
```