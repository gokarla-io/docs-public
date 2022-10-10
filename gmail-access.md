# Offline Access to Gmail users problem


## Business case

- periodically scan and read user emails to extract tracking information.




## Existing authenticate flow implementation

- App users authenticate through firebase and gets userId, userToken and refreshToken.
- The backend validate user tokens throw firebase python package firebase_admin.

    Firebase  <> App <> Backend



## Problem:

- Firebase provides only refresh token to the backend which is not enough to get the offline access to gmail. "Client Id" & "Client Secret" are needed.


## Question(s):

- How can we get the access with the existing auth. flow in place?


