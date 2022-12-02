# Adno demo

## Get started with ADNO

Adno is a web application to visualize, edit and a peer-to-peer sharing for static high quality pictures.

ADNO has 2 available versions : a Full version including the Editor and Viewer and the Light one including only the Viewer.

## How to start with ADNO ?

First, go to [ADNO Repository](<https://github.com/Serli/adno/releases/latest>) and download the version you would like to use (FULL or LIGHT)

Unzip the ADNO package

In order to use the app on your machine, you need to use a web server

Go to your folder containing ADNO and can create a light web server

You can use this command to run a web server on the port 8080

```
python -m http.server 8080
````

Enjoy using Adno !


# Licence



# IIIF pictures examples
    * https://ronallo.com/iiif-workshop/presentation/example-manifests.html
    * https://free.iiifhosting.com/iiif/1c8d49343676a04fffcd92979c02e9394e48bac96f590fffbadffc9133cd06b9/info.json
    * https://iiif.emf.fr/iiif/3/peutinger.jp2/info.json
    * https://iiif.emf.fr/iiif/3/saint-savin.jpg/info.json


# For developpers

## Prerequisites

First, install *[NodeJS](https://nodejs.org/en/)* on your computer

Then, open a command prompt and you need to install the package manager **Yarn** with the command 

`npm install --global yarn`

## Starting procedure

If you want to contribute to ADNO here are few steps to start 
  * clone the project from github `git clone https://github.com/Serli/adno.git`
  * switch to **adno-react** branch `git checkout adno-react`
  * Start the project with the following command : **yarn start**
    * Create a **.env** file and put the version you would like to use by using the variable ADNO_MODE=FULL or ADNO_MODE=LIGHT

      If you are on Linux or MacOS

      **LIGHT VERSION** `echo "ADNO_MODE=LIGHT" > .env`

      **FULL VERSION** `echo "ADNO_MODE=FULL" > .env`

Copy the followings commands to your terminal : It will automatically clone the project from github, install all the required dependencies and finally start the project on <http://localhost:1234>



```
git clone https://github.com/Serli/adno.git
cd adno
git checkout adno-react
yarn start
```


## Build procedure
```
yarn build-light
```

```
yarn build-full
```


## Manage Errors
In case of getting errors, there are some solutions.

You can try to :
  * Remove node_modules folder

    ```
      rm -r node_modules
    ```
  * Remove cache from parcel
    ```
      rm -r .parcel-cache
    ```
  * Remove yarn.lock
    ```
      rm yarn.lock
    ```

  Copy all commands
    ```
      rm -r node_modules
      rm -r .parcel-cache
      rm yarn.lock
      yarn start
    ```


# Hosting 

## Host ADNO with Github Pages

Download the latest release of Adno with the version of your choice ( full-version or light-version) from  https://github.com/Serli/adno/releases/latest

Unzip the archive to your folder and push it to your Github repository.

Once you’ve pushed to Github you need to go to Github’s website, select your repository and click on the “settings” tab.

Then, select the tab “Pages” on the left panel.

You’ll have to select the branch you want to deploy the website from and save your choice.

Enjoy using Adno !


## Hosting ADNO with Netlify

Create an account on Netlify

Create a project on Netlify

Build your project from **yarn build-full** for the full version and **yarn build-light** for the light version.

Upload your build folder to Netlify

