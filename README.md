## Introduction Of Docsify
Docsify is a tool that helps you easily make documentation websites using simple text (Markdown). It makes your documentation look nice, with features like easy navigation, search, and different themes. To use it, you install Docsify on your computer and follow a few quick steps to set up your documentation.

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

## Markdown Usage ##

>Docsify uses Markdown to format your documentation content. Markdown is a simple and easy-to-read language for styling plain text.

## Navigation and Sidebar ##

>In Docsify, navigation and the sidebar are essential for organizing and presenting your documentation effectively.

**Navigation:**
- Configuration:

- - Use the `nav` option in Docsify's settings.
- - Example: Customize the top navigation bar with specific links like Home, Guide, and API.

**Sidebar:**
- Configuration:
- - Use the `sidebar` option to structure the sidebar.
- - Example: Define the order and hierarchy of sections like Home, Guide, and API.

## Configuring and enabling the search functionality in Docsify: ##

>Enabling search functionality in Docsify involves a few simple steps:

>1.Configuration:

- - Open your Docsify configuration file (often named `index.html`).
- - Locate the configuration section.
- - Add a few settings for search, such as setting the cache duration and specifying paths to search.
  
>2. Search Box:

- - After enabling search, a search box will appear, typically in the top right corner of your documentation site.

>3.User Interaction:

- - Users can type search queries into the search box.

>4.Dynamic Results:

- - As users enter more characters, Docsify will display dynamic results below the search box.

> Navigation:

- - Users can click on search results to navigate directly to the corresponding section of your documentation.

## How to integrate Docsify with GitHub: ##
>Install Git 

```bash
sudo apt install git
```
>Check git Version

```bash
sudo apt --version
```
>Output

```bash
apt 2.4.11 (amd64)
```
>Create a New Repository:

- Navigate to the local project directory:

```bash
cd Desktop/Docsify2
```

- Initialize a new Git repository:

```bash
git init
```

- Add file in your git repository:
  
```bash
git add index.html
git add README.md
git add doc.txt
```
- Git commit

```bash
git commit -m "first commit"
```
>Output

```bash
[main (root-commit) 7d616d7] first commit
 3 files changed, 88 insertions(+)
 create mode 100644 README.md
 create mode 100644 doc.txt
 create mode 100644 index.html
```
>Git Push

```bash
git push origin main
```
## Github Link ##

```bash
https://github.com/Sanjit242001/Docsify.git
```

## List of Pluings ##

  **Emoji**

- Renders a larger collection of emoji shorthand codes. Without this plugin, Docsify is able to render only a limited number of emoji shorthand codes.

- Deprecated as of v4.13. Docsify no longer requires this plugin for full emoji support.

```bash
<script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/emoji.min.js"></script>
```

**External Script**

- If the script on the page is an external one (imports a js file via src attribute), you'll need this plugin to make it work.

```bash
<script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/external-script.min.js"></script>
```
**Zoom image**

- Medium's image zoom. Based on medium-zoom.

```bash
<script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/zoom-image.min.js"></script>
```
