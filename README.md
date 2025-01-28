# Codespirals

A GitHub repository to upload and save reusable, broadly generic projects that can be integrated into other projects to reduce code duplication.

### Libraries:
A codespirals library is a set of code made for a specific purpose, which is usually described by the module's name and README.
#### Structure
* Codespirals libraries usually contain anywhere from one to all of the following submodules, depending on size and scope:
  * Shared
    * Collections of interfaces that dictate the outline and behaviour of objects
  * Frontend
    * A set of classes and interfaces building upon the "Shared" package to facilitate the use of the module in a frontend application. 
  * Backend
    * An as generically-as-possible implemented set of the interfaces from the "Shared" package to facilitate adding the module to a user's EF Core database and generally using it in backend code.

### Solutions:
A codespirals solution is a set of code with full functionality that solves some requirement, which can be implemented into a project.
#### Structure
* A solution contains all necessary Interfaces, Entities, Models to achieve its goal, as well as:
  * Options
    * Most solutions also contain an "option" POGO class which will be injected into the services of the solution, which dictates the options that can be set that will later be read by the solution code
  * App builder extensions
    * A set of extensions to simplify adding the the solution's services to the builder (usually "Program.cs" file)

## Current generic codespirals packages:
### Libraries
* Base - A few basic interfaces that simplify some basic actions and classes. ☭🔑 Progress: 100% (In testing)
* Api - A set of extensions and code to streamline building an API. ☭🔑 Progress: 40%
* Users - Unified user handling for smaller projects. ☭🔑 Progress: 100% (In testing)

### Solutions
* Mail - A service to very easily implement mailing in any project. ☭🔑 Progress: 90%
* ApiCaller - A service to standardize calling an API from code. ☭🔑 Progress: 100% (In testing)
* Scheduler - A package to easily add a Quartz task scheduler to a project. ☭🔑 Progress: 70%
* Pay - A lightweight solution to implement payment in a project (currently only supports Stripe). ☭🔑 Progress: 80%


## Misc
### Symbols
* ☭ completly open source. free to fork, modify and use for anyone however they wish
* 🔓 open source, but with an attribution licence
* 🔑 private until fully tested and released
* 🔒 private with no current plans to release publicly
