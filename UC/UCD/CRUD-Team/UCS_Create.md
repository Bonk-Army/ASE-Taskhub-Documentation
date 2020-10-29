# TaskHub
## Use-Case Specification: Create a Team  v. <1.0>

## 1. Use-Case Create a Team

### 1.1 Brief Description
In this UC we describe, how an Admin can create a new Team.

## 2. Flow of Events
Needs to be done....later
__picture must be inserted__

### 2.1 Basic Flow
The Basic flow of this UC is, that an admin creates a new Team which is a group of users. He needs the name of all Users. Every other variable gets generated automatically. He also needs to repeat the Teamname so there is no misstyping. If the two names match the new Team gets written to the Database.

### 2.2 Name not met the conditions
 __picture must be inserted__

### 2.2 Repeated Name
The name exists in the Database. We send an alert message to the admin, that the name is already into the DB, and he must choose another name. We believ that a Teamname is *unique*.
 __picture must be inserted__

### 2.3 Name with "unrecognizable" Characters
If the name contains a non ASCII Letter, we send an alert message dialog to the admin, that the name contains unrecognizable characters, and can not be written into the DB.
 __picture must be inserted__

## 3. Special Requirements
### 3.1 User needs to be an Admin
The user must have the needed rights as an admin to create a Team.

## 4. Preconditions
### 4.1 User needs to be logged in
The user needs to be authenticated, to get the specific user rights.

## 5. Postconditions
### 5.1 New Class is created
A new Team is created in the DB and accesable in the Admin GUI.
 __picture must be inserted__
  
## 6. Extension Points
![FP](https://raw.githubusercontent.com/Unk3wn/TaskHub---Documentation/main/UC/UCD/CreateAClass/FP_CreateAClass.png)
