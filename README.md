

# Petflix
My-Todos is a basic API built with ruby's Sinatra DSL. 

This project is a demo that shows the power of the DSL in building server-side applications quickly.

The application has been built with the MVC design pattern.

## Pre-Requisites
In order to use this repository you will need the following:



- Operating System **(Windows `10+`, Linux `3.8+`, or MacOS X `10.7+`)**
- RAM >= 4GB
- Free Space >= 2GB

## Built With
This application has been built with the following tools:

![ruby](https://img.shields.io/badge/Ruby-CC342D?style=for-the-badge&logo=ruby&logoColor=white)
![sqlite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)


- **Ruby `v2.7.+`**
- **SQlite3 `v1.6`**
- **ActiveRecord `v7.0.4`**
- **Rake `v13.0.6`**
- **Puma `v6.1`**
- **rerun `v0.14`**
- **Sinatra `v3.0.5`**
- **ERB `v4.0`**

## Setup
You can setup this repository by following this manual

1. Clone the repository
    ```{shell}
   git clone https://github.com/otsembo/my-todos-sinatra.git
   ```
2. Ensure the ruby gems are setup in your machine
    ```{shell}
   bundle install
   ```
3. Perform any pending database migrations
   ```{shell}
   rake db:migrate
   ```
4. Run the application
    ```{shell}
    rake start
    ```
5. Open the application from your browser
    ```
   http://localhost:9292
   ```
   
### MODELS
Database schema definitions.
1. `/pets/create` - Add a new TODO item.

   ```{json}
   ## REQUEST BODY
   {
    "title": "Tommy",
    "description": "Prepare milk and cereal",
    "image": "https://i.insider.com/5484d9d1eab8ea3017b17e29?width=1136&format=jpeg",
    "due": "2023-06-09"
   }
   ```
2. `/pets` - List all available PETS.

   ```{json}
   ## RESPONSE SAMPLE
   {
    "data": [
        {
            "id": 2,
            "title": "maxy",
            "description": "vaccinated small cat",
            "due": "2023-02-24T00:00:00.000Z",
            "createdAt": "2023-02-24T09:34:41.856Z",
        }],
    "message": "SUCCESS"
   }
   ```
3. `/pets/update/:id` - Update an existing TODO.
4. `/pets/delete/:id` - Delete a TODO item.
5. `/` - Render a table of all todos using Bootstrap and ERB



## LICENSE
This repository is distributed under the MIT License


## Author
This repository is maintained by:

- [Alex Tanui](https://github.com/otsembo) 