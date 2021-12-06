# Iteration 2 Identifying Structures to Support Primary Functionality
The outcomes of the actions undertaken in each of the ADD phases in the second iteration of the design process for the LinkedHub system are shown in this section. We go from the general and coarse-grained functionality descriptions used in iteration 1 to more comprehensive decisions that will drive implementation and, as a result, the establishment of development teams in this iteration.

## Step 2: Establish Iteration Goal by Selecting Drivers
The primary use cases and concerns for this iteration are:
  1. UC - 1
  2. UC - 2
  3. UC - 6
  4. CRN - 3
 
## Step 3: Choose One or More Elements of the System to Refine
In this iteration, we will be refining the server side of the application. It's important for the system to support connecting to both client and the server easily. The modules which are required are located in the server since we are utilizing the web Web Application Architecture.

## Step 4: Choose One or More Design Concepts that Satisfy the Selected Drivers
| Design Design and Locations | Rationale and Assumptions |
| --------------------------- | ------------------------- |
| Create a domain model for the application | Before starting the functional decomposition, we need to create an initial domain model of the system that identifies the key entities in the domain and their relationships. There are no good options. Finally, it is necessary to build a domain model. Otherwise, it won't happen in an optimal way, resulting in specialized architectures that are difficult to understand and maintain. After a series of brainstorming sessions, we were able to create a domain model for our project using er diagrams and schema diagrams. |
| Identify Business Logic and map it to the use cases | In order to appropriately segregate concerns and specify data processing, use cases must be mapped to business logic. Alternatively, functional needs might be mapped to business entities, but certain requirements could be overlooked, or the business workflow could be riddled with duplication.|
| Decompose Business Logic into Business Entities | The entities for the business domain and their business logic are represented by combined business entities. Decomposing business logic into business entities has no viable alternatives.|
| Use Ajax and PHP | Ajax stands for Asynchronous Javascript and XML. AJAX is basically a technique which reloads certain contents of the page without actually reloading the entire page. Whereas on the other hand, PHP is a scripting language that stands for hypertext processor. We’d be using PHP for most of our client-side processing and to connect the business logic to the server. |
