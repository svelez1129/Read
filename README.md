<!-- up to date as of June 6th 2024 -->
# Windows Setup (New)

This guide documents how to set install Replate on a Windows machine.

1. [Install Node.js](#install-nodejs)
2. [Install Yarn](#install-yarn)
3. [Install Ruby](#install-ruby)
4. [Install Rails](#install-rails)
5. [Install bundler](#install-bundler)
6. [Clone and Setup Replate-Business](#clone-and-setup-replate-business)
7. [Update Config](#update-config)
8. [Setup the Database](#setup-the-database)
9. [Start the Server](#start-the-server)

## Install Node.js

1. Download and install nodejs version 14.X from the offical website: https://nodejs.org/en/download/package-manager
2. Check the current nodejs version by running:
```shell
node -v
```

## Install Yarn
1. Install yarn by running
```shell
npm install -g yarn
```
2. Check if it is version 1.22.X
```shell
yarn -v
```

## Install Ruby
1. Install the ruby version corresponding to what is currently used: https://rubyinstaller.org/downloads/
2. Install ruby version 3.0.6
3. Check the current ruby version by running:
```shell
ruby -v
```

## Install Rails
1. Run the following:
```shell
gem install rails -v 6.0.6
```
2. Check to see if it was installed, it should be version 6.0.6
```shell
rails -v 
```

## Install bundler
```shell
gem install bundler:2.3.25
```

## Clone and Setup Replate-Business
1. Contact your project manager to provider you access to the [GitHub repository](https://github.com/replate/replate-business) and add you as a memeber of the [Replate Organization](https://github.com/replate).
2. Clone business repo:
```shell
git clone https://github.com/replate/replate-business.git
```

3. Navigate to the replate-business directory
```shell
cd replate-business
```

4. Run the following:
```shell
bundle install
yarn install
```

## Update Config

- Get `database.yml` and `application.yml` from an engineer or product manager
- Add them to the `config` folder

## Setup the Database 
- Run `rake db:setup`

## Start the Server
- Run `rails server`
