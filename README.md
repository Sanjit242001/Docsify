## Introduction Of Docsify
>Docsify is a tool that helps you easily make documentation websites using simple text (Markdown). It makes your documentation look nice, with features like easy navigation, search, and different themes. To use it, you install Docsify on your computer and follow a few quick steps to set up your documentation.

## Docsify Setup

**Requirement of docsify**

- PRETTY_NAME="Ubuntu 22.04.3 LTS"
- NAME="Ubuntu"
- VERSION_ID="22.04"
- VERSION="22.04.3 LTS (Jammy Jellyfish)"
- VERSION_CODENAME=jammy
- D=ubuntu
- ID_LIKE=debian
- HOME_URL="https://www.ubuntu.com/"
- SUPPORT_URL="https://help.ubuntu.com/"
- BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
- PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
- UBUNTU_CODENAME=jammy

## Requirement Tools ##

>Node.js<br>

>NPM

## Node.js ##

Node.js isn't directly used by Docsify, but it can be helpful when you're creating Docsify documentation. It helps you preview and test your documentation on your computer.

 >Download Node.js

```bash
sudo apt install Node.js
```

>Check Node.js version

```bash
sudo node -v
```

>Output

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
## Initialize ##
```bash
docsify init ./docs
```
>Output
```bash
Initialization succeeded! Please run docsify serve ./docs
```
## Preview your site ##

>Run the local server with docsify serve. You can preview your site in your browser on http://localhost:3000.

```bash
docsify serve docs
```
>Output
```bash
Serving /home/sanjit/docs now.
Listening at http://localhost:3000
```
## Markdown configuration ##

>docsify uses marked as its Markdown parser. You can customize how it renders your Markdown content to HTML by customizing renderer:

```bash
window.$docsify = {
  markdown: {
    smartypants: true,
    renderer: {
      link: function() {
        // ...
      }
    }
  }
}
```

>Configuration Options Reference: marked documentation

>You can completely customize the parsing rules.

```bash
window.$docsify = {
  markdown: function(marked, renderer) {
    // ...

    return marked
  }
}
```
## Navigation and Sidebar ##

>In Docsify, navigation and the sidebar are essential for organizing and presenting your documentation effectively.

**Navigation:**

>Alternatively, you can create a custom markdown-based navigation file by setting loadNavbar to true and creating _navbar.md, compare loadNavbar configuration.

<!-- index.html -->

```bash
<script>
  window.$docsify = {
    loadNavbar: true
  }
</script>
```

**Sidebar:**

>In order to have a sidebar, you can create your own _sidebar.md (see this documentation's sidebar for an example):

>First, you need to set loadSidebar to true. Details are available in the configuration paragraph.

<!-- index.html -->

```bash
<script>
  window.$docsify = {
    loadSidebar: true
  }
</script>
```

## Configuration ##

>You can configure Docsify by defining window.$docsify as an object:

```bash
script>
  window.$docsify = {
    repo: 'docsifyjs/docsify',
    maxLevel: 3,
    coverpage: true,
  };
</script>
```

>The config can also be defined as a function, in which case the first argument is the Docsify vm instance. The function should return a config object. This can be useful for referencing vm in places like the markdown configuration:

```bash
<script>
  window.$docsify = function (vm) {
    return {
      markdown: {
        renderer: {
          code(code, lang) {
            // ... use `vm` ...
          },
        },
      },
    };
  };
</script>
```

### alias ###

- Type: `Object`

>Set the route alias. You can freely manage routing rules. Supports RegExp. Do note that order matters! If a route can be matched by multiple aliases, the one you declared first takes precedence.

```bash
window.$docsify = {
  alias: {
    '/foo/(.*)': '/bar/$1', // supports regexp
    '/zh-cn/changelog': '/changelog',
    '/changelog':
      'https://raw.githubusercontent.com/docsifyjs/docsify/master/CHANGELOG',
    '/.*/_sidebar.md': '/_sidebar.md', // See #301
  },
};
```
## Themes ##

>There is a handful of themes available, both official and community-made. Copy Vue and buble website custom theme and @liril-net contribution to the theme of the black style.

```bash
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/themes/vue.css" />
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/themes/buble.css" />
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/themes/dark.css" />
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/themes/pure.css" />

```
## How to integrate Docsify with GitHub : ##

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
