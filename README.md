# dotFiles
These are the starter dotfiles used by cgiandi employees.

### Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

#### Prerequisites

You need to have Nodejs 6.x and Yarn installed to use these dotfiles.

##### For linux:

Installing node 6.x & yarn

```
curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
sudo apt-get update
sudo apt-get install -y nodejs yarn
```

##### For macOS:

Installing homebrew

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Installing node 6.x & yarn

```
brew update
brew install node@6 yarn
```

#### Installing

To use the eslint configurations you need to add the following to your project package.json

```
yarn add eslint 
        \eslint-config-airbnb 
        \eslint-plugin-import 
        \eslint-plugin-jsx-a11y 
        \eslint-plugin-react -D
```

Then you need to copy the content of eslint directory to your project base directory

```
cp -a eslint/. ~/workspace/<your_project>/
```
You also have to setup your code editor to use eslint as linter.

