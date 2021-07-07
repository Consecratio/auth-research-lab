# ![GA Logo](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Auth Research Lab

---

Authentication is a complex and exciting topic that involves using many of the concepts we've already studied as well as several new ideas. 

An authentication system allows the registration / signup of new users and allows those users to sign in. It has to be able to identify each user and keep their information private and secure.

Being able to develop secure user login systems is in fact a whole career and life path in and of itself, but understanding the broad concepts of **Auth** is critically import for all developers. 

Describing auth flow and understanding key terms are very common **interview questions** for junior developers, so lets take some time to research and understand auth and the related concepts.

## Setup

Fork and clone this repository and answer the questions as you research directly in the README. You do not have to pull request and submit this lab, but you will want to have it on hand for reference in the future. 

## Auth Concepts Worksheet

#### Define the following

1. *Authentication*
   - Authentication establishes the identity of the user to provide access to the application.
2. *Authorization*
   - Authorization determines what the user can do. (What do they have access to, what can they manipulate)
3. Explain how *authentication* and *authorization* are related but distinct concepts.
   - Authentication and Authorization are part of the security of the site each part coming together to allow users to utilize the site.
4. *Sessions vs Token based auth*
   - Sessions are stored utilizing cookies after a user has loged in. The cookie is sent with each request to verify the state after each request.
   - Token authentication creates a JSON Web Token which contains a secrete and is stored in the client's local storage. This token is sent in the header of each request and the server validates the token after each request.
5. *json web token (also know as a jwt)*
   - JWT is a token created by the server which contains a secret and then it is sent to the server in the header of each request, and then the server must check if the JWT is valid before responding.
6. *Encoding, encryption and hashing* along with the uses for and differences between the three
   - Encoding transforms data so that it can be properly consumed by a different type of system. It is not used to keep information secret, but to ensure that it's able to be properly read.
   - Encryption transforms data in order to keep it secret from others. It is used to keep information secret from parties who are not supposed to view the data.
   - Hashing ensures integrity so that we know if the data has been changed. Hashing takes in any input and produces a fixed-length string that should, in theory, always come out the same if the input is the same. So if you hash a password typing that same password should give you the same hash.
7. *oAuth* (pronounced oh-Auth)
   - oAuth is an open standard for access delegation used as a way for users to grant websites or applications access to their information on other websites but without giving them the password. It provides clients a secure delegated access to server resources on behalf of resource owners.

#### Explore and then describe the following npm packages:

1. [bcrypt](https://www.npmjs.com/package/bcrypt)
   - A library used for hashing passwords.
2. [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken)
   - A library used for creating, signing, and decoding JWTs.
3. [passport](https://www.npmjs.com/package/passport)
    * also describe what a *strategy* is in the context of this npm package
   - Passport is used for authenticating in express. Strategies are different ways that Passport can handle authentication and how it will react to those different situations.

---

## Licensing
1. All content is licensed under a CC-BY-NC-SA 4.0 license.
2. All software code is licensed under GNU GPLv3. For commercial use or alternative licensing, please contact legal@ga.co.
