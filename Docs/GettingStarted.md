# Getting Started
## Overview
This document is designed to help a new developer setup their machine to start development for this repo. 
This will go over the most basic instructions.

## Step 1: Get `nvm`
### How do I know if I have `nvm`?
Run this in your terminal:
``` bash
nvm --version
```
If that returns with a `Command 'nvm' not found` then you know you don't have it. 

### How do I get it?
You can always just go to the `nvm` repo and follow their guide: https://github.com/nvm-sh/nvm

To keep it simple though, just run this command:
``` bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```
Afterwards, open and close your terminal so you can start using `nvm`.

You can double check if `nvm` installed correctly by running `nvm --version` again and it should return with a version number.

## Step 2: Install NodeJS 12.4.0
Currently, we're using NodeJS version `12.4.0`. If we update the version, you'll be alerted.

Anyways, run this command in the terminal:
``` bash
nvm install 12.4.0
```

That should install the correct node version. You can double-check that by running the following command:

``` bash
nvm ls
```

That should list the available node versions you have on your machine. `v12.4.0` should be on that list. 

### Set your node version
You have installed `v12.4.0` but you probably haven't set it as the version to use. To do that, run the following command:
``` bash
nvm use 12.4.0
```
You might get an error that says 
``` bash
$ nvm use 12.4.0
$ nvm is not compatible with the npm config "prefix" option: currently set to "/home/nik/repos/nvm/versions/node/v12.4.0"
$ Run `nvm use --delete-prefix v12.4.0` to unset it.
```
... in which case, all you need to do is literally run this command:
``` bash
nvm use --delete-prefix v12.4.0
```

### Check if you are on the right version of NodeJS
Now run this command in the terminal:
``` bash
node --version
```
It should be `v12.4.0`!

## Step 3: Verify `npm`
Make sure you have `npm` installed as well. This should already be installed, but you can verify with the following command:
``` bash
which npm
```
If you have `npm` installed, then you'll see something like this:
``` bash
$ which npm
$ nvm/versions/node/v12.4.0/bin/npm
```

## Step 4: Get ReactJS
