---
# Vue.js Starter: vue-runner
## Professional Vue.js Development Setup for Complete Beginners
---

## Node Ecosystem Install:
** *Setup Explained:* ** Node is a server writing in the JavaScript language.  We will install Node locally on your machine (used by Webpack) to improve the development experience when you are building your Vue.js apps.
<br>

### Install Node and n:

(Skip if you have Node and npm already installed)

> $ `curl -L https://git.io/n-install | bash`
>
> For further information: `https://github.com/mklement0/n-install`

### *Optional*: Install and use n to install a "stable" version of Node:
** *Note*: **  "n" is a "node version manager" which allows you to install different versions of Node (or use "nvm" an alternative to "n").  This is helpful to make sure you have the latest version, and can change versions of Node as needed while building apps in the JavaScript community.  If you have a recent version of Node, this will likely not be necessary to use our Vue.js `vue-runner` project.
> 
> **Install n:** (From: https://github.com/tj/n):
> <br>
> $ `npm install -g n`
> <br>
> $ `n stable`


### *Alternatively*, Install and Update Node, npm, and n manually:
>   **See Node install instructions:** 
>
>   `https://nodejs.org/en/`
>
>   **Update NPM:**
>   
> $ `sudo npm install npm -g`
>
>   **Install n:** (From: `https://github.com/tj/n`):
>   
> $ `npm install -g n`
>
>   **Use n to install a 'stable' version of Node:**
>
> $ `$ n stable`


---
# Vue.js "Vue-Runner" Quick Starter

---

## Clone repo to get copies of all branches:

> **Clone the repo:**
> 
> $ `git clone https://github.com/kobione/vue-runner.git`
>
> ** *Note* **: clones only 'master' branch, by default.
> <br>
>
> **Change into vue-runner/ directory:**
> 
> $ `cd vue-runner/`
> <br>
>
> **Note that, at first, you only have 1 branch:**
> 
> $ `git branch`
> <br>
> Should see only 'master' branch
>
> **Run this bash script to get local copies of 3 *new* branches:**
> <br>
> *(master branch + 3 more branches)*
> 
> $ `git branch -a | grep -v HEAD | perl -ne 'chomp($_); s|^\*?\s*||; if (m|(.+)/(.+)| && not $d{$2}) {print qq(git branch --track $2 $1/$2\n)} else {$d{$_}=1}' | csh -xfs`
>
> ** *Alternatively*,** you can grab branches individually.
> <br>
>
> **Check to verify that you have all branches:**
> 
> $ `git branch`
> <br>
> Should see master branch + 3 more branches.

<br>


## Install Dependencies:
**NOTE:** Our project it dependent on vbuild, and npm packages.
<br>Must install vbuild and run `npm install` for each branch to run properly.
<br>

### **Install vbuild:**

> **Use npm to Install vbuild Globally:**
> 
>  $ `npm i -g vbuild`
> <br>
> vbuild is a great tool to quickly build Vue.js apps.
> <br>
> For more information, and *alternative install instructions* check out: `https://github.com/egoist/vbuild`
> <br>

### **Install npm packages:**
> 
>  $ `npm install`
> <br>
> **Note:** May be package duplication via vbuild and npm packages. This is known. 

---
# Select One of Vue-Runner's 3 Branches:
---

## **Start our Application:**

> For any of our branches, you can run:
> 
>  $ `npm run dev`
> <br>
> ** *Note:* ** Must stop & start server, if you switch branches.
> <br>
>
>  **Launch your browser and go to:** [http://localhost:4000/](http://localhost:4000/)
<br>


## **Use one of Vue-Runner's 3 starter branches:**


### `master` branch is currently *SAME* as Branch 3: `single-file-component`.

- It is suggested that if you want to use any one branch moving forward, you **delete**  your copy of `master` branch and create a new "master" by branching off of whichever one of the 3 branches you prefer to use.
<br>

## Branch Names, plus Branch Descriptions and Instructions:

> ### *Branch1:* 1-simple-vuejs
>
>   - Only two files: `index.html` and `scripts.js`
>     <br>
>   - $ `npm run dev` to launch local Python server
>     <br>
>          **-OR-** open file: `index.html` in your browser.
>     <br>
>
>   **Note:** No Webpack, will need to manually refresh browser after each "save" in editor.
> 
<br>

> ### *Branch2:* 2-vuejs-autoreload
>
>   ** *Errors??*: **  If you are trying to launch the server by typing $`npm run dev`
>     and you see red errors in your terminal, try typing $ `npm install` again.
>  
>   - Two files: `index.html` and `src/main.js` plus Webpack
>     <br>
>   - When you "save" in your editor, will automatically reload browser
>     <br>
>   **Note:** The Webpack build tool auto-reloads your page, and is used to do much more.
> 
<br>

> ### *Branch3:* 3-single-file-component
> 
>   - Use in Production: HTML, CSS, and JavaScript combined in one .vue
>     <br>
>     ** *For example*: ** The HTML, CSS, and JavaScript in `App.vue` bundles together into one component
>     <br>
>     <br>
>     **Note:** Use single file "components" to build components out of other, smaller components
>     <br> 
>   - When you "save" in your editor, will automatically reload browser (thanks to Webpack)
>     <br>

---