
# Item Catalog
This web application is a project for the Udacity FSND Course.

## Project Overview
This application  provides a list of items within a variety of categories
as well as provide a user registration and authentication system.
Registered users will have the ability to post, edit and delete their own items.

## Software	Installation

   * Vagrant:	https://www.vagrantup.com/downloads.html
   * Virtual Machine:	https://www.virtualbox.org/wiki/Downloads
   * Download	a	FSND	virtual	machine:	https://github.com/udacity/fullstack-nanodegree-vm
   After downloading requierd software you can access VM by e	following	commands:
      1) cd vagrant
      2) vagrant	up
      3) vagrant	ssh
      4) cd	/vagrant
      5) cd catalog
      6) Setup application database python database_setup.py
      7) Insert fake data python lotsofitems.py
      8) Run application using python catalogApp.py
      9) Access the application locally using http://localhost:5000

## 	Using Google Login
To enable Google login in the app. the following steps requierd:

 1)	Go to Google Dev Console
 2)	Sign up or Login if prompted
    3)	Go to Credentials
    4)	Select Create Crendentials > OAuth Client ID
    5)	Select Web application
    6)	Enter name 'catalog'
    7)	Authorized JavaScript origins = 'http://localhost:5000'
    8)	Authorized redirect URIs = 'http://localhost:5000/login' && 'http://localhost:5000/gconnect'
    9)	Select Create
    10)	Copy the Client ID and paste it into the data-clientid in login.html
    11)	On the Dev Console Select Download JSON
    12)	Rename JSON file to client_secrets.json
    13)	Place JSON file in catalog directory
    14)	Run application using python catalogApp.py


## JSON Endpoints
    The following JSON are open to the public:

    /categories/JSON - Displays all categories.

    /categories/<int:categories_id>/item/JSON - Displays a specific category with its item
  
    /categories/item/JSON - Displays all categories with its items
