Mangopay Node.js SDK
=================================================
MangopaySDK is a Node.js client library to work with
[Mangopay REST API](http://docs.mangopay.com/api-references/).


Installation
-------------------------------------------------
Install the module via npm

    npm install mangopay2-nodejs-sdk --save

Usage inside your app

    var mangopay = require('mangopay2-nodejs-sdk');
    
    var api = new mangopay({
        clientId: 'your_client_id',
        clientPassword: 'your_client_password'
    });
    
    api.Users.create(...)

License
-------------------------------------------------
MangopaySDK is distributed under MIT license, see the 
[LICENSE file](https://github.com/Mangopay/mangopay2-nodejs-sdk/blob/master/LICENSE).


Unit Tests
-------------------------------------------------
Mocha tests are placed under ``/test/`` folder


Contacts
-------------------------------------------------
Report bugs or suggest features using
[issue tracker on GitHub](https://github.com/Mangopay/mangopay2-nodejs-sdk).

Account creation
-------------------------------------------------
You can get yourself a [free sandbox account](https://www.mangopay.com/signup/create-sandbox/) or sign up for a 
[production account](https://www.mangopay.com/signup/submit-your-app/go-live/) (note that validation of your production 
account can take a few days, so think about doing it in advance of when you actually want to go live).


Configuration
-------------------------------------------------


Sample usage
-------------------------------------------------
Don't forget to check examples folder !
    
### Creating a user ###

    mangopay.Users.create({
        "FirstName": "Victor",
        "LastName": "Hugo",
        "Address": "1 rue des Misérables, Paris",
        "Birthday": 1300186358, 
        "Nationality": "FR",
        "CountryOfResidence": "FR",
        "Occupation": "Writer", 
        "IncomeRange": "6", 
        "ProofOfIdentity": null,
        "ProofOfAddress": null, 
        "PersonType": "NATURAL", 
        "Email": "victor@hugo.com", 
        "Tag": "custom tag",
    }, function(model) {
        // User created - using callback
    }).then(function(model){ 
        // User created - using promise
    });;


Sample usage of Mangopay SDK installed with npm in a Node.js project
-------------------------------------------------
Don't forget to check examples folder !

Logging
-------------------------------------------------