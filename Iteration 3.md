# Iteration 3: Addressing  Quality Attribute Scenario Driver (QA-3) 

## Step 2
The goal of this iteration is to focus on QA-5.A user is able to upload information about themselves to create a profile within the server during normal operation. The user will send the data to the server which will be checked for any inappropriate words or phrases, then uploaded to the database. Any other user should be able to see the changes made when reviewing the user’s profile within 1 minute of uploading.

## Step 3
For this iteration, the elements that have been chosen to be refined are: 
  1. Database server
  2. Application server

## Step 4
| Design Decisions and Location | Rationale and Assumptions |
| ----------------------------- | ------------------------- |
| Implement a sampling management system for the rate of data from the database | Reducing the stream of data will greatly increase the performance of the database, thus reducing delay on requests for crucial operations such as adding a new registered user |
| Introduce the load balancing switches tactic within the application server |HTTP requests can become a mess for a server if it’s attempting to handle many at one time. For the solution, load balancing switches are implemented to handle where the request should be redirected thus improving performance | 

## Step 5
| Design Decisions and Location | Rationale |
| ----------------------------- | --------- |
| Initializing load balancing switches tactic on separate server | Initializing the load balancing tactic upon separate servers, external from the database and application server and allow for proper request redirection that doesn’t affect the performance of data requests |
| Use sampling management system tactic for application and database servers | Implementing this tactic upon our servers will increase performance greatly as it reduces the amount of requests for data due to the frequency of data being decreased. Overall, the performance of the servers would be increased |

## Step 6
[Refined Deployment Diagram]()

## Step 7


