UC - AssignStudent
=========================

Activity Diagramm
-----------------
![Activity Class](https://raw.githubusercontent.com/Unk3wn/TaskHub---Documentation/main/UC/UseCases/AssignStudent/AssignStudent.png)

[Cucumber Testcase](https://github.com/Unk3wn/TaskHub---Codebase/blob/master/CucumberTests/src/test/resource/AssignStudent.feature)
----------------
        Feature: Assign Student
          AS an Admin
          I want to assign an Student/User to an class

          Scenario Outline: Add Student to class
            Given : The user is logged in
            Given : User is an Admin
            Given : The user is on the Updatepage of the Adminpanel
            When : I choose an <class> out of an Dropdownmenu with the id 'classes_menu'
            Then : <class> Updatepage opens
            When : I enter <studentname> into input field with the id 'studentname_input'
            And : I click the button 'Add to Class' with the buttonid 'add_to_Class'
            Then : <status>-Popup with <message>

            Examples:
              | class     | studentname | status | message |
              | TINF19B4  | Nico        | OK     | Student added to class |
              | TINF19B5  | NULL        | ERROR  | Error : Student not found |

          Scenario: Good Case
            Given : The user is logged in
            Given : User is an Admin
            Given : The user is on the Updatepage of the Adminpanel
            When : I choose an <class> out of an Dropdownmenu with the id 'classes_menu'
            Then : <class> Updatepage opens
            When : I enter <studentname> into input field with the id 'studentname_input'
            And : I click the button 'Add to Class' with the buttonid 'add_to_Class'
            Then : "OK" Message

          Scenario: Good Case
            Given : The user is logged in
            Given : User is an Admin
            Given : The user is on the Updatepage of the Adminpanel
            When : I choose an <class> out of an Dropdownmenu with the id 'classes_menu'
            Then : <class> Updatepage opens
            When : I enter <studentname> into input field with the id 'studentname_input'
            And : I click the button 'Add to Class' with the buttonid 'add_to_Class'
            Then : "OK" Message
