Download Link: https://assignmentchef.com/product/solved-cse-106-lab-5
<br>



Create a grades program that has a similar functionality to the one you created in Lab 1, but this will be a web application. For this lab you will create the user interface with HTML, CSS, and JavaScript which will make requests to an existing backend service to fulfill the requests. Your web application should:

<ul>

 <li>Allow a user to ask for a grade from the backend and display the grade, given the student name</li>

 <li>Allow the user to see all students and grades</li>

 <li>Allow a user to create a new student name and grade in the backend</li>

 <li>Allow a user to edit a grade in the backend</li>

 <li>Allow a user to delete a grade in the backend</li>

</ul>

The REST API you will use has the following methods at https://amhep.pythonanywhere.com:

GET /grades

Input: None

Return: JSON of students with grades

GET /grades/&lt;student name&gt;

Input: None

Return: JSON of student with grades

POST /grades

Input: JSON of student name and corresponding grade, e.g. {“name”: “John Doe”, “grade”: 92.1}

Return: JSON of student with grades after operation takes place

PUT /grades/&lt;student name&gt;

Input: JSON of the grade that corresponds to the student name in the URI, e.g. {“grade”: 92.1}

Return: JSON of student with grades after operation takes place

DELETE /grades/&lt;student name&gt;

Input: None

Return: JSON of student with grades after operation takes place

Be aware:

<ul>

 <li>This code will be used again for the next two labs, so make it good</li>

 <li>Please don’t upload inappropriate names as this is shared by the whole class  Please don’t delete all the names for the same reason</li>

</ul>

Hints:

<ul>

 <li>Student names are case sensitive in URI and JSON</li>

 <li>Use %20 instead of a space in the URI since spaces aren’t allowed and represented by %20</li>

 <li>POST and PUT requests should have the header Content-Type: application/json</li>

</ul>