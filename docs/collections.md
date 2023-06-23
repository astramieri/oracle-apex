# APEX Collections

Collections enable you to store rows and columns currently in the session state so that they can be accessed, manipulated, or processed during a user-specific session. Just think of collection as a bucket in which you temporarily store a name rows of information.

Every collection contains a named list of data elements or members, which can have up to:
- 50 character attributes - VARCHAR2(4000)
- 5 number attributes
- 5  data attributes
- 1 XML type attribute
- 1 large binary attribute (BLOB)
- 1 large character attribute (CLOB). 

You insert, update, and delete collection information using PL/SQL API APEX_COLLECTION.

## Usecase

When you are creating a data entry wizard in which multiple rows of information, first needs to be collected within a logical transaction. The user can make many updates apply these updates to a collection, and then call a final process to apply the changes to the database.

