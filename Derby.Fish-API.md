# Derby.Fish-API
## Codebase
The API server is written in the Rust programming language using the Axum framework.

## Project Structure
The project is broken up into seperate modules each defining objects needed to make up the codebase.

### main.rs
Main Entry point, this essentially defines top level modules and initializes an instance of the HTTP server.

### db.rs
All function and structres related to working the the database connection.

### middleware.rs
Functions to provide valuable information using the components of a request. This happens when a request is recieved and is used for authentication filtering and other basic request modifications.

### schema.rs
This is a diesel generated file that defines the diesel structures necessary to work with our database.

### server.rs
Functions and structures regarding the operation of the axum server.

### traits.rs
Traits and their associated structs and implementations to be used for making our codebase more reusable and coherent.

### resources.rs
A module that contains submodules to create HTTP handlers for all the resources our app deals with.

### models.rs
A module that contains submodules that define the Rust type defenitions and their implemented functions for each database table.
