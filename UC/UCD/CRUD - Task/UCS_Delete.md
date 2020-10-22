# TaskHub
## Use-Case Specification: Delete new task  v. <1.0>

## 1. Use-Case Delete new task

### 1.1 Brief Description
In this UC we describe, how an user can delete an existing task.

## 2. Flow of Events
Needs to be done....later
__picture must be inserted__

### 2.1 Basic Flow
The Basic flow of this UC is, that an user deletes an existing task object in our persistent Database. He needs the task object to delete it. The teacher can only deletes tasks which he created and which are for a class which are assigned to him.

### 2.2 Name not met the conditions
 __picture must be inserted__

## 3. Special Requirements
### 3.1 User needs to be an Admin
The user must have the needed rights as a teacher to delete a task.

## 4. Preconditions
### 4.1 User needs to be logged in
The user needs to be authentificated, to get the specific user rights. He also have to be a teacher, just the users with a teacher role have the access to delete a task.

## 5. Postconditions
### 5.1 Task is deleted
The task will be updated as "deleted" in the DB and it is not yet accesable for the teacher and for the assigned class.
 __picture must be inserted__
  
## 6. Extension Points

**n / a**