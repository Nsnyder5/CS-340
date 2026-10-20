# CS-340

## Grazioso Salvare Rescue Dashboard

This repository contains my Project Two work for CS 340 Client/Server Development. The project involved developing a database-driven dashboard for Grazioso Salvare, an organization that identifies dogs that may be good candidates for search-and-rescue training.

The application uses MongoDB to store and retrieve Austin Animal Center outcome data and Python to provide access to the database. The dashboard was created using the Dash framework and includes interactive filtering options, a data table, a breed visualization, and a geolocation map.

## Maintainable, Readable, and Adaptable Programs

I try to make programs maintainable, readable, and adaptable by separating different responsibilities into reusable components, using descriptive names, adding comments where they are helpful, and avoiding unnecessary duplication. One example of this approach was the `CRUD_Python_Module.py` file created during Project One. Instead of writing MongoDB connection and database commands directly into every application, I created an `AnimalShelter` class that contains the create, read, update, and delete operations.

This approach made Project Two easier because the dashboard could import the existing CRUD module and use its methods to communicate with MongoDB. The database logic and the dashboard interface remained separate, which made the program easier to understand and modify. It also meant that changes to the database access code could be made in one location instead of throughout the dashboard.

In the future, the same CRUD module could be reused as the data-access layer for other applications that need to interact with the animal shelter database. For example, it could support another dashboard, a reporting application, an API, or an administrative program. The class could also be expanded or adapted to work with additional collections or database requirements.

## Approaching Problems as a Computer Scientist

When approaching this project, I first broke the client's requirements into smaller technical problems. Grazioso Salvare needed access to animal shelter data, specific rescue-animal filtering options, an interactive data table, and visualizations that changed with the selected data. I treated the database, data-access module, dashboard controls, and visualizations as separate parts that needed to work together.

I began with the database and CRUD functionality before developing the user interface. I then created queries that matched the client's rescue requirements and connected those queries to the dashboard controls using callbacks. After each major feature was added, I tested it before moving to the next part of the project. This was different from some earlier programming assignments because I had to think about the entire application rather than only solving one isolated programming problem.

For future database projects, I would use a similar process. I would begin by identifying the client's data and functional requirements, design the database structure and access methods, implement reusable code for interacting with the data, and then build the user-facing components. I would also test each component independently before testing the complete application. This approach helps make problems easier to manage and makes it easier to identify errors.

## What Computer Scientists Do and Why It Matters

Computer scientists use software, data structures, databases, algorithms, and other technologies to solve problems and improve how people work with information. Their work matters because software can turn large amounts of raw data into information that is easier to understand and use when making decisions.

In the Grazioso Salvare project, the original animal shelter data contains thousands of records. Searching through those records manually would be inefficient. The dashboard gives the organization a way to filter the data according to different rescue categories and immediately view matching animals in a table, chart, and map.

This type of application could help Grazioso Salvare identify potential rescue-training candidates more efficiently. Instead of manually examining every record, employees can use the filtering and visualization tools to narrow the data to animals that meet particular requirements. A well-designed system can reduce the amount of time required to analyze data, improve consistency, and allow the organization to focus more of its resources on its rescue mission.

## Project Technologies

- Python
- MongoDB
- PyMongo
- Dash
- Plotly
- Dash Leaflet
- Pandas
- Jupyter Notebook
- Codio

## Repository Contents

- Project Two dashboard source code
- CRUD Python module developed in Project One
- Project Two README documentation
- Project Two submission files
