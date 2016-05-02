# Shift Cipher
##### An message encryption web app made in Drupal.

#### By Ryan Brown

## Description

This site allows users to enter a phrase and have it encrypted depending on a number chosen between 1 and 25, and a direction of either right or left.  Entering in "hi there!", with a shift value of "1" and a direction of "right" will result in "ij uifsf!".  Each letter has changed into the letter just right of its position in the alphabet ("h" is now "i" and so on).  Changing the number to two would have turned "h" into "j".

If the input was the number "1" with a direction of "left", the letter "h" would turn into its left neighbor in the alphabet, "g".  And so on.

The ancient Romans used this as a means to encrypt secret messages...pretty cool!

This was built in a custom module complete with form validation, leaving no room for user error.  Hope you enjoy!

## Setup

* Clone repository from `https://github.com/browneryan/shift-cipher-drupal` and navigate to directory
* Open MAMP (or WAMP) application, select preferences, change document root to the bookstore folder
* A browser window should open upon success (if not click open start webpage), then click the tools tab and select phpMyAdmin
* Choose import tab, click choose file button and select the database zip file within sites/db-backup folder named `bookstore.sql.zip`
* The database name is `bookstore`
* Click on database name and select privileges tab, then select add user
* Set username to `admin`, host to `localhost`, and set password to `admin` as well
* Make sure 'grant all privileges on database' is checked, then click go
* Open a new browser tab to `localhost:8888`
* Login username and password are both `admin`
* Reviewer role username and password are both `reviewer`
* Test authenticated user username and password are both `user`
* Alternative to entering in each role's username and password, you can use the Masquerade block found in the first sidebar

## Technologies Used

* Drupal
* PHP

### Legal

Copyright (c) 2016, Ryan Brown

This software is licensed under the MIT license.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
