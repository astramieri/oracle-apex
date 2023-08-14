# Authentication

Authentication is the process of establishing each user's identity before they can access your application. 

It may require a user to enter a username and password or it could involve the use of digital certificates or a secure key.

If all the users have the same rights and privileges, they are referred to as **public users**.

In APEX you can choose from the following authentication methods:
- built-in preconfigured authentication scheme
- creating a custom authentication scheme (you must implement a PL/SQL function)
- choosing to not require authentication

## Preconfigured Authentication Schemes

0. No Authentication
1. Oracle APEX Accounts
2. Custom Authentication
3. Database Schema Accounts
4. HTTP Header Variable
5. Open Door Credentials
6. LDAP Directory
7. Oracle Application Server SSO Server
8. SMAL Sign-In
9. Social Sign-IN

## How Authentication Works

You determine how your application interacts with users. If all users have the same rights and privileges, they are referred to as public users. However, if your application must track each user individually, you must specify an authentication method.

Authentication establishes the identity of each user who accesses your application. Many authentication processes require that a user provide some type of credentials such as a user name and password. These credentials are then evaluated and they either pass or fail. If the credentials pass, the user has access to the application. Otherwise, access is denied.

Once a user has been identified, the Application Express engine keeps track of each user by setting the value of the built-in substitution string APP_USER. As a user navigates from page to page, the Application Express engine sets the value of **APP_USER** to identify the user. The Application Express engine uses APP_USER as one component of a key for tracking each user's session state.