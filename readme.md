# Template for Lumen Microservice# Lumen PHP Framework

## How to install it
`composer create-project --prefer-dist hanga/pkg_back_meta_package_lumen ms_<MICROSERVICE_NAME>`

* `mkdir ms_<MICROSERVICE_NAME>`
* `composer global require "hanga/pkg_back_meta_package_lumen"`
* `git init`
* `git add .`
* `git commit -m "Initial commit" `
* `git push -u origin master`


## Working Tree
```
   app/
    |---- Console/
        |--- Commands       -> Commands
    |---- Exceptions        -> Error Handling
    |---- Http
        |--- Controllers
        |--- Middleware     -> MiddleWare
    |--- Jobs               -> Manage queuable functions
    |--- Models
          ├── Business/     -> Contains all the logic
          ├── DataAccess/
            ├── Read        -> Contains the functions that read the data
            ├── Write       -> Contains the functions that write the data
          ├── Entities/
            ├── Eloquent    -> Contains the eloquent model
          ├── Transformers/ -> Defines the output data structure
    |--- Providers

    config/
    |--- databases.php      -> Contains the 4 empty connections: `persons`, `monitoring`, `core`, `organization`
```