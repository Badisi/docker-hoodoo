# hoodoo

This **docker image** aims to deliver a tailored environment for web projects development.  

## What's inside ?

This image include the following dependencies :

- nvm
- node
- yarn
- yo
- plop
- electron
- angular-cli
- java
- maven
- git

## How to use it ?

**Prerequisites** :   

- (mandatory) a running docker environment   

- (optional) public SSH keys if you need authentication

- (optional) an X-Server for graphical support

**Getting started** :   

1. Download and modify the **hoodoo** script provided in this repository   

   ```javascript
   // mandatory
   - WORKSPACE : "path to your local workspace (ie. where the source code of your web projects resides)"

   // optional (only if you want to benefits from your local maven cache)
   - M2 : "path to your local .m2 folder"

   // optional (only if you need authentication)
   - SSH : "path to your local .ssh folder"

   // optional (only if you need graphical support)
   - X11 : "possible values are 'mac' or 'win'"
   ```

2. Run the **hoodoo** script   

   ```bash
   > sh hoodoo
   ```

## How to upgrade it ?

1. Remove any previous docker image or container from your system  

2. Run the **hoodoo** script   

   ```bash
   > sh hoodoo
   ```  

## Bonus : run GUI applications

**macOS platform**   

1. Download and install [XQUARTZ](https://www.xquartz.org/)   

2. Restart your computer   

3. Modify the **hoodoo** script as follow:

   ```bash
   X11="mac"
   ```
4. Remove any previous docker image or container from your system   

5. Run the **hoodoo** script   

   ```bash
   > sh hoodoo
   ```  

**windows platform**   

1. Download and install an X-Server   

2. Restart your computer   

3. Modify the **hoodoo** script as follow:

   ```bash
   X11="win"
   ```
4. Remove any previous docker image or container from your system   

5. Run the **hoodoo** script   

   ```bash
   > sh hoodoo
   ```  
