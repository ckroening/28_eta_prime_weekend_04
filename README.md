# eta_prime_weekend_04

Welcome to your fourth weekend challenge!

This week we will combine your knowledge of Node, Express, Mongo, jQuery, and Bootstrap!

Overview
Rando Corp. is ready to launch its very first Web application to

accept applications from talent online
search and view those applications
When applicants visit the homepage, they will see an empty form that allows them to submit an application to Rando. That data will be stored in a MongoDB collection, named `applications`.

Rando admins can view applicant data by going to the homepage and clicking on the "Admin" button or navigating directly to /admin. Once an admin gets to the page, they see the latest applications they've received. In addition, admins can search by name, skills, and/or location to find applicants that match their criteria.

There is no need to secure the admin page with a password at this time.

Details
Home Page (index.jade)

Components

Header
Rando Corp name to left
Button to access admin page to the right
Body with employment form
Employment form fields
First name
Last name
Desired job
Desired location
Remote
Specific Location
City
State
Employment history will take up to three jobs
Job title
Employer
City
State
Description of duties
Skills
Footer with Rando Corp
Event Handling

When form is submitted data should be POSTed to a /applicant route and saved to the database
Admin Page (admin.jade)

Components

Header
DIsplays "Rando Corp Applicant Admin"
Search form
Provides ability to search applicant data by name and/or desired location and/or skills
Matching Applicants table
A table of applicants that match the searched criteria, displays all results
Pre-search, it should just show the last 5 applications that have been submitted
Available data
First name
Last name
Desired location
Last employer
Skills
Event Handling

Search form submission
Perform a GET on /admin/search with query parameters (client-side)
Respond with JSON that has the results and the desired data to display in the Matching Applicants table
You will get this data by performing a server-side query of Mongo
Update the DOM with the received data
Database

For this application, you will only need one collection: applications. You will need to store all of the applicant's data:

First name
Last name
Desired job
Desired location
Remote
Specific Location
City
State
Employment history will take up to three jobs
Job title
Employer
City
State
Description of duties
Skills
You will also want to capture the date the application was received.

Bootstrap

Use the bootstrap grid to create your page content and use two or more other Bootstrap styles and/or features to style your page.

Hard Mode
Implement the ability to sort each column of the applicant's table. For example, the table might have a table heading with each field name. When I click on a field name the first time, the data is sorted in ascending order; the second time, the data is sorted in descending order.

Pro Mode
Implement the ability for applicants to edit their previously submitted applications.
