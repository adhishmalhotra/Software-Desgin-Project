# Iteration 1: Establishing an Overall System Structure
Here is the [full pdf]() of iteration 1 
## Step 1: Review Inputs

| Category | Details |
| ------------- | ------------- |
| Design purpose  | This is a Social Networking website. The purpose of this is to produce sufficiently detailed design to support the functionality of the website. The system should provide the user the ability to create an account, login into their account, search for different users in the database or different posts in the system, add/remove friends, share/delete posts, modify their profile, etc. |
| Primary Functional requirements |  Of the use cases presented in Figure 1.1.1, the primary ones are: - UC -1 because it is the first step in accessing the website - UC - 2 because it directly supports the core functionality  - UC - 6 because it directly supports the core functionality 
| Quality attribute scenarios | The scenarios which are explained above are prioritized in the following table: <img src=“images/iteration1QAs.jpg” raw=true style=“margin-right: 10px;” />
| Constraints |All constraints are included as drivers. 
| Architectural Concerns | ID Concern CRN-1 Accomplish completion of the final system in the allotted time and resources. CRN-2 Evenly distribute the workload within the project across the development team to fully utilize the team's capabilities. CRN-3 Creating the first prototype model of the system’s structure. CRN-2 was selected as the driver.

## Step 2: Establish Iteration Goal by Selecting Drivers  
The drivers that will be focused on in this iteration are:
  1. QA-1: Performance
  2. QA-2: Availability
  3. QA-5: Usability
  4. QA-6: Security
  5. QA-7: Security
  6. CON-1: A user isn’t able to create a collaboration project with only themselves.
  7. CON-3: Any changes to projects, profiles, or any other user change on the machine must be recorded.
  8. CON-4: The server must be accessed using one of the following web browsers (Chrome V3.0+, Firefox V4+, IE8+) and the only acceptable platforms being Windows,OSX, and Linux.
  
## Step 3: Choose One or More Elements of the System to Refine
In this iteration, we will be refining the server side of the application. It's important for the system to support connecting to both client and the server easily. The modules which are required are located in the server.

## Step 4: Choose One or More Design Concepts that Satisfy the Selected Drivers
| Design Design and Locations | Rationale |
| -------------- | ------------- | 
| Logically structure the client part of the system using the Web application reference architecture | Web application reference architecturesupports deploying and running our application on a web browser. It is fairly easy to create views for a web application as compared to any other type of Web application reference architecture application. Choosing this architecture itself supports QA-3, QA-4, QA-5. Moreover, it also supports CON-3 and CON-7. |
| Discarded Alternatives:|  Alternative Reason for discarding Mobile Application This alternative was discarded because this type of device was not considered for accessing the system. |
| Logically structure the server part of the system similar to a web application | The database which is created for the purpose of this application is primarily used for storing different types of data that would be essential to our application. Most of the processing is done before-hand, meaning the data which is supplied by the user is first checked to make sure whether it’s relevant or not, and once it's established that the data is relevant, it’s stored in the database. The application follows a client-side scripting pattern. All of the team members are familiar with the MySQL database system and hence we decided to proceed with this architecture specifically. |
| Physically structure the application using the three-tier deployment pattern | The three tier development pattern is used because the web application requires a browser that the user connects from for the client, a server that is used for the logic, and finally a dedicated server only for the data that is inputted on the application. | 
| Discarded Alternatives: | A two tier development pattern was considered but was found to be insufficient due to the data having to remain on its own server. Furthermore, a tier development pattern over 3 would be too many as it’s not required. |
| Build the user interface of the client application using HTML, CSS, bootstrap, JQuery, JavaScript and PHP | Building the user interface on the foundational blocks of HTML, CSS, bootstrap, Jquery, Javascript, and PHP provides a great outlook for the project as each one provides some aspect of workability upon the user interface. | 
| Discarded Alternatives: | React was discarded due to its complexity and learning curve. Angular was also discarded for the same reason of its complexity and the learning curve that comes along with it. The team of development felt more comfortable working with the frameworks listed above. | 
| Deploy the application using GitHub Pages | GitHub Pages allows you to turn GitHub repositories to create websites. All the changes are made and pushed in real time, which will allow changes to projects, profiles, or any other user change on the machine to be recorded. (CON-3) GitHub pages support more than 750 MME types hence, the deployed website will be accessible on many different browsers including Chrome V3.0+, Firefox V4+, IE8+. (CON-4)|

## Step 5: Instantiate Architectural Elements, Allocate Responsibilities and Define Interfaces
| Design decisions and Location | Rationale |
| ------------------------------ | --------- |
| Create initial domain | Initial domain model helps understand working of the system |
| Define modules based on Use case model | Business logic made using the reference from the use case model |
| Incorporate a separate layer to hold the data on server side | Adding a third layer to the server side that will manage the data ensuring that it is consistent with the data on the dedicated server.|
| Connecting the database access module to data source | The data layer that exists on the server side will have access to the database through an access module. The purpose of this module is to provide access to the SQL database server. |

## Step 6: Include all Rough Diagrams
## Step 7: Design the Kanban Board

