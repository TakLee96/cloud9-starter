How to use Cloud9?
==================

##Getting Started##

* Go to [Cloud9](http://c9.io) to register an account and log in.
* Go to the Dashboard page and select **Create New Workspace** -> **Create a New Workspace**
* Give your workspace an awesome name, and select **Hosted** and **Custom**
* After Cloud9 has processed your workspace, select it on the left panel and click **START EDITING**
* In the new tab, this is what you will see: ![Oops](http://i60.tinypic.com/2djs5s1.jpg)
  * The files are shown on the left of the page
  * Opened files are shown in the middle of the page
  * The Terminal can be found on the bottom of the page
  * You can also click the "**+**" to open up a new tab
  * You can drag the terminal window up to make it bigger
  * Tabs can be dragged to the left, right, upper or lower section
* You can now play around with this new IDE. Happy Coding!

##Setting up the Environment##

* To set up the Cloud9 environment to run our Ruby application, we need to complete a few steps. Please type or copy-and-paste each command in your terminal and watch it run completely. If there is any error occured, please contact me at [jiahang_li@berkeley.edu](mailto:jiahang_li@berkeley.edu). Please be patient, as some commands might a while to complete:
  * ```curl https://raw.githubusercontent.com/saasbook/courseware/master/vm-setup/configure-cloud9-1.1.2.sh > configure-cloud9-1.1.2.sh```
  * ```bash --login configure-cloud9-1.1.2.sh```
* You are now ready to do the homework :)

##Homework##

* To start with a new homework, please copy the github link
* Make sure the terminal says "**~/workspace**" for your current directory
* In the terminal, type: ```git clone [the github link]```
* After git has downloaded the homework, the new folder should display on the left
* In the terminal, type: ```cd [the name of the new folder]```
* In the terminal, type: ```bundle install```
* If the gems are not previously installed, you might need to wait for a while for the gems to be downloaded and installed

##To Run Your Application##

* Whenever you want to run your Rails application, please use this command in the terminal: ```rails s -b $IP -p $PORT``` (You can find a detailed documentation about running your Rails application [here](https://docs.c9.io/v1.0/docs/running-a-rails-app))
* There will be a small window like this: ![Oops](http://s24.postimg.org/b6hzkiz83/2015_07_07_10_33_45.png)
* If you click on the link, it's going to take you to the preview of your app
* You can also copy the link and view it in your own browser

##Heroku Deployment##

* Make sure you have your heroku account and password ready, otherwise please go to [heroku](https://signup.heroku.com/www-header) and sign up for a new account
* In the terminal, do ```heroku login``` and enter your email and password
* Make sure you are in the homework folder and then do ```heroku create```
* To deploy your application to heroku, simply do ```git push heroku master```
* For more about heroku deployment, please vist [heroku](https://devcenter.heroku.com/articles/getting-started-with-ruby#deploy-the-app)
