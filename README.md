# cosc349-assignment1
Git Repository for COSC349 Assignment 1

The application runs using a three Virtual Machine (VM) setup. One VM is setup and named webserver, this is the first VM running a web page that is given to the staff to enter details of newly purchased assets and send through to the database by submitting the form. The second VM runs a database using MySQL that stores the information on assets entered by responsible staff for each Departments. The third VM runs a web server again providing the interface for administrator, in this case the Asset Management Team to review and approve of the information received. This third web page could be used to run reports of new assets purchased each month or year and could be extended to provide ease of tracking of assets for the Office.
Virtual Machines
webserver
ip address: 192.168.56.11

dbserver
ip address: 192.168.56.12

adminserver
ip address: 192.168.56.13

All three virtual machines are running Linux Ubuntu. The ‘webserver’ VM provides the user with a web interface to enter details of newly purchased assets. The ‘dbserver’ VM runs a database (MySQL) storing the entered data. The ‘adminserver’ is basically a web interface for admins to view the updated entries into the database.
To run and use this application:
Open a terminal or command prompt on windows and enter the following command,
git clone https://github.com/ezra24/cosc349-assignment1
Navigate to the folder you cloned the repository in, making sure the Vagrantfile is in that folder and run the following command:
vagrant up
Once all the updates and scripts are done running. All three virtual machines or all three servers are now available to use. Access the first webserver via http://192.168.56.11 and basically go from there

