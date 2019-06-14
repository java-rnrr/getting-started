---
layout: post
title: "Week 1 Beginner: Setting Up"
description: If you need to configure your computer for use with FTC start here! 
---

### Date: Saturday June 8th, 2019
* Everyone created GitHub accounts
* Those with PCs installed git bash
* Used git to download the repository containing bashrc & bash_profile


### Setting Up

* [Download Android Studio][android-install]

### Setting up Android Studio

Add steps here..


# How to Install JDK and Android Studio
* The Android Studio Tutorial in the link below shows you how to download Android Studio in Section 9
  * [FTC Android Studio  Programming Training Manual](https://www.firstinspires.org/sites/default/files/uploads/resource_library/ftc/android-studio-tutorial.pdf)
* Alternatively, watch the following video and follow the additional instructions listed below:
  * [FTC Tutorials: Android Studio Setup and Installation](https://youtu.be/uTjYo9w0TaY)
     * The Android Studio Install and Setup Guy talks too fast, so turn on closed-captioning (CC) and use the settings to change the speed to 0.75 or 0.5, so the guy talks slower
     * Go to the JDK Download site below: http://www.oracle.com/technetwork/java/javase/downloads/index.html
     * Select the JDK Platform (JDK) at the top, then it will ask you to click on the "Accept License Agreement check box under the Java SE Development Kit 10.0.2. Then click on the jdk-10.0.2_xxx, for your corresponding device.
     * Then go thru the installation process for JDK
     * Android Studio Download: https://developer.android.com/studio/index.html
     * Click the Download button, then click the "I have read terms and conditions..." and click Download button.
     * Then click on the downloaded file and drag it to applications.
* You must disable Android Studio Instant Run shown in Section 9.2 of the Android Studio Tutorial because it can cause difficult-to-troubleshoot problems with Android Studio.
  * On the Android Studio launch window, click on Configure->Settings in the bottom right corner. Then go to the "Build, Execution, Deployment" on the left panel of the Settings window and click on the "Instant Run" on the left panel. Then uncheck the "Enable Instant Run..." check box to disable "Instant Run".

# How to Create a GITHUB account
* Go the the following website: [How to Create an Account on GitHub](https://www.wikihow.com/Create-an-Account-on-GitHub)
  * Select a username that you would like to use for this account. Make sure you write it down or remember it!!!
  * Select an email address.  I recommend you use your yourname@rocknrollrobots25.com email, but if you prefer you can use another email address, just remember which one. This email is important since it is the one that will receive your activation email with a link to activate the account, so don't pick an email that you cannot log into!!!
  * Select a password and make sure you remember it!  (the password must contain at least one lowercase letter, one number, and seven characters)
  * Read the GitHub Terms of Usage and Privacy Policy and talk to your parents if you don't understand or have any questions
  * Press the "Create an account" button
  * Choose the personal plan: "Unlimited public repositories for free"
  * You do NOT need to click on the "Help me set up an organization next"
  * Click the Continue button
  * Answer the "How would you describe your level of programming experience?" question
  * Answer the "What do you plan to use GitHub for?" and select "Other" (you can select the other boxes also if they apply)
  * Answer the "Which is closest to how you would describe yourself" with "I'm a student"
  * Then press the Submit button
  * GitHub will send you an activation email (to the email you supplied earlier) with a ink to activate the account.  Just click the URL link in the email that you receive
  * Congratulations! You should have successfully created your GitHub account!

# How to Setup Your .bashrc and .bashrc_profile
* Make FIRST directory
  * mkdir ~/Desktop/FIRST
* Change to the FIRST directory
  * cd ~/Desktop/FIRST
* Download java-rnrr/software 
  * git clone https://github.com/java-rnrr/software.git
* Change directory into 'software' directory
  * cd ~/Desktop/FIRST/software
* Copy .bashrc and .bash_profile files to home directory 
  * Copy bashrc to ~/.bashrc
    * cp bashrc ~/.bashrc
  * Copy bash_profile to ~/.bash_profile
    * cp bash_profile ~/.bash_profile
  * Only .bashrc is run on non-login shells, while only .bash_profile is run on login shells.
    * .bash_profile    
      * When you log in .bash_profile is executed to configure your shell before the initial command prompt
      * .bash_profile should contain things that need to be defined at login time only, like PATH and other environment variables, startup programs, etc. You just need things once, not in every shell you open. In most cases, you also need the things from .bashrc in your login shell. That's why .bash_profile sources .bashrc as well, but .bashrc doesn't usually source .bash_profile.
    * .bashrc
      * But, if you’ve already logged into your machine and open a new terminal window (xterm) then .bashrc is executed before the window command prompt. .bashrc is also run when you start a new bash instance by typing /bin/bash in a terminal.
      * .bashrc should typically contain things you want to set in every shell you open, like aliases, functions, etc. These are per shell session items that are not inherited from environment.
  * Determine your user name
    * echo $USER
  * Now edit the ~/.bashrc file and remove the '#' at the beginning of the 'export' line and replace REPLACE_WITH_YOUR_USER_NAME with your user name
    * vi ~/.bashrc


Done! You're ready to move on the Lab 1!

[android-install]: https://developer.android.com/studio
