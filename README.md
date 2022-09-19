# Library Management Portal
Library Management Portal is a web-based application using ASP.NET and SQL that provides the ability to find books, manage books, borrow books, track borrowed books. It automates most of the library activities for librarians and students.
Go to the application: http://librarymanagementportal.somee.com

Features for the librarian (admin):
1. Author management: add, update, or delete the authors
2. Publisher management: add, update, or delete the publishers
3. Book Inventory: add, update, or delete books
4. Book Issuing: manage the issued books for the users
5. Member Management: manage members
6. View Books: view all books in the system
7. Login: login for admin (Admin ID: admin, password: admin)

Features for the users:
1. User Profiles: manage users profiles
2. View Books: view all books in the system
3. User Sign up: sign up to be member
4. User login: login for members (Ex: Member ID: member1, password: member1), (Ex: Member ID: member2, password: member2)

Steps to test this application on your local computer:
1. Download this project: https://drive.google.com/file/d/1VH9xqL92ueqE4466Wlqrl1XCASDOCd91/view?usp=sharing
2. Extract it then open Visual Studio
3. Go to File -> Open -> Project/Solution -> open LibraryManagementPortal.sln
4. Restore database using the backup database file in database folder from the extracted project
   - Copy the backup database file in database folder from the extracted project and paste in C:\Program Files\Microsoft SQL Server\MSSQL15.SQLEXPRESS\MSSQL\Backup (based on where you installed SQL Server)
   - Open SQL Server Management Studio then connect to your local server
   - Right click Databases -> Restore database
   - Choose device -> click ... -> add -> click the backup database file -> ok
5. Go to web.config and change the connection string with the new one
   - Go to Visual Studio -> View -> Server Explorer -> Connect to database -> choose Microsoft SQL Server -> continue
   - Copy and paste your local database server name
   - Go to Connect to a database -> click the dropdown -> select the database -> click test connection to test it first -> ok
   - Go back to Server Explorer then click the connection in Data Connections
   - Copy the connection string in Properties window
   - Paste it to connection string in web.config
6. Right click homepage.aspx in Solution Explorer -> Select as Start Page
7. Run the project
