# TaskHub
## Use-Case Specification: Create new task  v. <1.0>

## 1. Use-Case Create new task

### 1.1 Brief Description
In this UC we describe, how an user can create a new task.

## 2. Flow of Events
Needs to be done....later
__picture must be inserted__

### 2.1 Basic Flow
The Basic flow of this UC is, that an user creates a new task object in our persistent Database. He needs a name of the new task, a class which should do the task and a deadline. For the teacher, he can only create tasks for a class which are assigned to him.

### 2.2 Name not met the conditions
 __picture must be inserted__

### 2.2 Repeated Name
The name exists in the Database for this class. We send an alert message to the teacher, that the name is already into the DB, and ask him if he really want to add the same task again.
 __picture must be inserted__

### 2.3 Name with "unrecognizable" Characters
If the name contains a non ASCII Letter, we send an alert message dialog to the teacher, that the name contains unrecognizable characters, and can not be written into the DB.
 __picture must be inserted__

## 3. Special Requirements
### 3.1 User needs to be an Admin
The user must have the needed rights as a teacher to create a task.

## 4. Preconditions
### 4.1 User needs to be logged in
The user needs to be authenticated, to get the specific user rights. He also have to be a teacher, just the users with a teacher roles have the access to create a new task.

## 5. Postconditions
### 5.1 New Task is created
A new task is created in the DB and accessible for the teacher and for the assigned class.
 __picture must be inserted__
  
## 6. Extension Points

**n / a**
