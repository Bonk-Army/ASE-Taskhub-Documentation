# TaskHub
## Use-Case Specification: Update a solution  v. <1.0>

## 1. Use-Case Update a solution

### 1.1 Brief Description
In this UC we describe, how an user can update an existing not submitted solution.

## 2. Flow of Events
![Flow](https://raw.githubusercontent.com/Unk3wn/TaskHub---Documentation/master/UC/UCD/CRUD-Solution/AD_Update.png)

### 2.1 Basic Flow
The Basic flow of this UC is, that an user updates an existing solution object in our persistent Database. He needs the solution object to update it and the changes. The teacher can only update solutions from his team.

### 2.2 Name not met the conditions
 __picture must be inserted__

## 3. Special Requirements
### 3.1 User needs to be an Admin
The user must have the needed rights as a team member to update a task.

## 4. Preconditions
### 4.1 User needs to be logged in
The user needs to be authenticated, to get the specific user rights. He also have to be a team member, just the users with a team member role have the access to update a solution.

## 5. Postconditions
### 5.1 New Task is created
The solution will be updated in the DB, and the changes are accessible for the teamledader and for the team member.
 __picture must be inserted__
  
## 6. Extension Points

**n / a**
