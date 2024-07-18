# Backend Challenge Spring 2024

As part of the challenge you will have to fork this repository and add your backend application in the forked version of this repository. You can find more information on how to fork a repository [here](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo).

If you have any questions about this challenge, please do not hesitate to reach out to Miguel Merlin [mmerlin@stevens.edu](mmerlin@stevens.edu).

## Challenge Overview
Challenge Details
Your task is to develop a CRUD application that adheres to the following specifications and requirements:

Application Overview
Purpose: Create a backend service that Creates, Reads, Updates, and Deletes volunteers from a database.
Technology Stack: You are free to choose the technology stack (programming languages, database systems, frameworks) that you are most comfortable with.
CRUD Operations
Create: Implement functionality to add new records to your database. For example, adding a new volunteer.
Read: Develop methods to retrieve and display records from the database. This could include listing all volunteers or searching for a specific user.
Update: Allow for modifications to existing records, such as updating a volunteer's contact information.
Delete: Provide a way to remove records from the database safely.
Volunteers Table
Field Name	Data Type	Description	Example
volunteer_id	UUID / INT (PK)	Unique identifier for each volunteer.	123e4567-e89b-12d3-a456-426614174000
first_name	VARCHAR	Volunteer's first name.	John
last_name	VARCHAR	Volunteer's last name.	Doe
email	VARCHAR	Volunteer's email address.	john.doe@example.com
phone_number	VARCHAR	Volunteer's phone number.	+1234567890
date_of_birth	DATE	Volunteer's date of birth.	1990-01-01
address	VARCHAR	Volunteer's address.	123 Main St, Anytown, AS
skills	VARCHAR / ARRAY	List of volunteer skills.	["First Aid", "Counseling"]
availability	JSON / VARCHAR	Volunteer's availability (could be structured as JSON).	{"Monday": ["AM"], "Saturday": ["PM"]}
date_joined	DATE	Date when the volunteer joined.	2024-03-21
background_check	BOOLEAN	Indicates if a background check has been completed.	true / false
Volunteers
List Volunteers

GET /api/volunteers
Retrieves a list of all volunteers, with options for pagination, filtering, and sorting.
Create a New Volunteer

POST /api/volunteers
Creates a new volunteer record.
Get Volunteer Details

GET /api/volunteers/{volunteerId}
Retrieves detailed information about a specific volunteer.
Update Volunteer Information

PUT /api/volunteers/{volunteerId}
Updates an existing volunteer's information.
Delete a Volunteer

DELETE /api/volunteers/{volunteerId}
Deletes a specific volunteer's record.
