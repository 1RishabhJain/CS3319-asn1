# CS3319-asn1

Instructions

Assignment 1
Objectives:
Upon completion of this assignment, you should be able to:

read a situation/scenario that describes data  and  then represent a model of the data and the relationships between the data using and ER diagram
map your ER diagram to a relational database.
insert nodes into a B+ tree given the order of the B+ tree
NOTE: you MUST have signed up with kritik.io in order to complete this assignment!
Part 1:
Draw the complete Entity Relation Diagram for the following scenario:

The city of London needs to keep track of its blood bank and clinics. Here is the information they need to store 

The blood types - each blood type has a unique number between 1 and 8, a type (one of A, B, AB or O), a RH factor (either + or -) and a percentage of people who have that type. Note: there are 8 types of blood, no more, no less.
The donor information - unique number, first name, last name, address (street, city, prov, postal code) and cell phone number. 
The clinic information - a unique clinic number, address (street address,  city, province, postal code) and phone numbers (at least 3 voices phone numbers)
The appointment information - a unique appointment number, a date, a time 
The staff information - a unique staff number, first name and last name, and cell phone number.
Also keep track of the following relationships:
Each donor has a blood type. Some blood types might not have any donors yet of that blood type
Each donor makes an appointment.  An appointment doesn't exist unless some donor made one. Donors cannot be in our system unless they made at least one appointment.
An appointment happen at  a clinic.  Every appointment must happen at some clinic. All clinics have had appointments. 
A clinic stocks blood. Keep track of how much of each type of blood is currently in stock. Also have a true or false field that is called NotEnoughInStock. Every clinic stocks blood. Not all blood types are in stock at every clinic. 
Staff members works at clinics. A staff member can work at many different clinics, keep track of the first day they worked at this clinic. When staff start initially, they have not been assigned a clinic. All clinics must have at least 3 staff members working at them. 
One staff member is the head of each clinic. Every clinic must have a head staff member.  Keep track of the date that staff member became head.  A staff member can only be head of ONE clinic, not more than one. 
Clinics call donors trying to encourage them to donate. Keep track of the last date the clinic called the donor.  A clinic might have never called any donors and some donors have not been called yet. Many clinics might call the same donor who has rare blood type.
If I have not explicitly stated something, then there is an obvious choice. Do not add any extra relationships that you assume should exist, just include the ones mentioned above.

Show both the cardinality of the relationships (the 1:M notation on the lines) and the participation (include both the (min, max) constraints AND the double line/single line notation). Do NOT include any extra information than is given above to illustrate the above database. For each entity, underline the key you would pick to be the primary key (if it is a weak entity, remember to use a dashed underline), if there is more than 1 candidate key, underline the key you would pick to be the primary key but make all possible candidate keys red (including the one you pick as primary). The underling will indicate which attribute was chosen as the primary key .

You will be marked on choosing the best solution, some solutions may work but not be the best! Do NOT use the Crows Foot Notation.

Use draw.io, MS Visio, or some other software that create E-R diagrams to create your E-R Diagram. Do NOT hand draw it. If you use draw.io, to create a pdf do File>Print and then select the .pdf.

Part 2:
Map Your Entity Relation Diagram to a Relational Database conceptually (you don't have to make it in an actual DBMS, just visually represent it), showing all tables, column heading, keys (primary and foreign, indicate if the key is primary with an underline and/or foreign with a star). You may use MS Word to draw the tables, or MS Access and then take screenshots of the tables. Do NOT hand draw it. Just give the names you would give to each table and the names for the fields. It should basically be the top row of each of the tables required to turn your ER diagram from Part 1 into a relational database but do not include any data, just the column/field headings.   For example, if you were making a relational database for a University, you would need a PROFESSOR table and a TEACHES table and I would want you to hand in something like this:

![pic](https://user-images.githubusercontent.com/45084203/136593097-38f6f230-693f-459b-bf7f-da7f7f4e237a.jpg)


Make sure you include ALL the tables required to map your ER diagram in part 1 to the relational database.

Part 3:
NOTE: This part can be hand drawn. First, write down the numbers 1 to 10 and write your answers to the following 10 questions next to the numbers at the top of a sheet. Then start to show the insertion of your answers into the tree as you insert your answers into the tree IN THE ORDER YOU ANSWERED THE QUESTIONS AS SHOWN BELOW.  You must go to left for <= in the tree and to the right for > .  Use the first letter(s) of each word (and then second letter and third letter and so on, if necessary, e.g. Ant comes before Apple)  to decide where in the tree they should go and ignore the case.  Start with an an initially empty B+-tree with 2 keys and 3 pointers per node. As you start the steps to insert your answers into the tree, in step 1, you should show the root node with the your answer to question 1 into the root node, then in step 2, you should show you inserting the word that is the answer to question 2, etc...You must show each step as the tree is being built. Put a horizontal line between each step.  Make sure you show the tree with the actual word(s) in it at each step, NOT a numerical representation of the words. Show the tree after the insertion of each item. Remember to show ALL pointers on every step (show NULL pointers as an O with a line through it, ie. Ø) and show the Hard Disk on every step.

What is your first name?
What is the name of the country in which your grandmother was born?
What is your favourite fish or animal that lives in the water?
What is the name of a country you would love to visit someday? 
What is your favourite vegetable ?
What is the name of the month in which you were born?
What is the name of your favourite TV show?
What is the name of your most hated vegetable?
Which animal are you scared of?
What is the course code of your favourite first year course (e.g. CS1026)
 
