# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


**Step 1: Install Ubuntu Desktop**
1. First and formost, let's install ubuntu desktop in the VM
    With the use of this link (https://ubuntu.com/download/desktop)
2. Crerate a new Ubuntu Server 20.04 desktop as per the instruction of Asssignment 3
3. Now Click on START Button to begin
4. After that just wait until it's finish the setup for UBUNTU DESKTOP VM
5. Let's setup Account for UBUNTU DESKTOP VM, so that you can able login in it
6. Upon completion of setup, hit ENTER when it display hit enter to eject/reset
7. After reboot, you need to enter account details (ID and Password) for login your account on VM


**Step 2: Ubuntu Desktop configuration and Setup**
1. Once it done,open the TERMINAL in the Ubuntu Desktop and Run the following Commands
 1. `$ sudo apt-get update`
 2. `$ sudo apt-get upgrade -y`
 3. `$ sudo apt-get dist-upgrade -y`
 4. `$ sudo reboot`


**Step 3: Jetbrains RubyMine IDE**
1. Open this link (https://www.jetbrains.com/ruby/download/#section=linux)
2. After finishing download it
3. Downloads the folder from the PaasProject folder and Extract it
4. Just leave it right now


**Step 4: Curl Installation**
1. Now we are going to install **CURL** in Ubuntu desktop 
 1. `$ sudo apt-get install curl`


**Step 5: RVM Installation**
1. Now we are going to install **rvm** in Ubuntu desktop 
 1. `$ gpg2 --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB`
 2. If you not able to run the above command because of missing package for gnupg2 that's why run the command
    1. `$ sudo apt install gnupg2`
 2. If you get an error just run the following command again
    1. `$ \curl -sSL https://get.rvm.io | bash -s stable`
 3. To start next part using **RVM** you need to run the following command
    1. `source /home/user/.rvm/scripts/rvm`
 4. Just to check version of **RVM** 
    1. `$ rvm -v`
 
 
**Step 6: Ruby Installation**
1. Now we are going to install **Ruby** in Ubuntu desktop 
 1. `$ rvm install ruby 2.6.6`


**Step 7: Bundler Installation**
1. Now we are going to install **bundler** in Ubuntu desktop 
    1. `$ gem install bundler`
 
 
**Step 8: Rails Installation**
1. Now we are going to install **rails** in Ubuntu desktop 
    1. `$ gem install rails`


**Step 9: Git Installation**
1. Now we are going to install **git** in Ubuntu desktop 
    1. `$ sudo apt-get install git`


**Step 10: Setup PaaS Project**
1. Now we are going to use that folder we extract before from the PaasProject.
2. After that we are going to work on Terminal and PaaSProject folder
    1. `$ cd Downloads/PaaS_Code`
3. After getting the path run the following command
    1. `$ rvm install $(cat .ruby-version) && rvm $(cat .ruby-version) do rvm gemset create $(cat .ruby-gemset) && rvm gemset use $(cat .ruby-gemset) && bundle install --jobs=$(nproc)`
4. Run the following command again
    1. `$ bundle install`
    2. `$ rails server`
    3. `rails db:migrate`
    4. `$ rails db:seed`
5. After finishing all of this just complete the steps to finish the setup


**Step 9: Heroku Deployment**
1. In this step, we are going to deploy the files from github
    1. `$ get config --global user.name "<Your Name Here (Vishva Shah)>"`
    2. `$ get config --global user.email "<Sample Mail ID Here (W0784026@myscc.ca)>"`
    3. `$ git init`
    4. `$ git add -A`
    5. `$ git commit -m "<Commit Description>"`
2. After geting all of these just run the following website
    (https://www.heroku.com/)
3. Run the followig commands to deploy your project to Heroku
    1. `$ curl https://cli-assets.heroku.com/install-ubuntu.sh | sh`
    2. `~/Downloads/PaaSProject$ heroku login`
4. After this, you have to login the Heroku accound
5. After that you can see the 5o articles with 10 commnets each are seeded.

**Finally the Paas Project is completed**
