Okay, I've updated the changelog to include more detail and the team members' contributions.# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to Semantic Versioning.

## [Unreleased]

## [1.0.0] - 2025-04-25
### Added
-   **General**
    -   Basic services source code (Marius Preda)
    -   Unit tests for the most used services (auth + db interact) (Marius Preda)
    -   DB visualisation (Marius Preda)
-   **Auth Service:**
    -   Implemented user authentication (registration, login) functionality. (Marius Preda)
    -   Added MongoDB for user data storage. (Marius Preda)
    -   Integrated mongo-express for database management. (Marius Preda)
    -   Added unit tests (Marius Preda)
-   **DB Interact Service:**
    -   Basic functionalities of database interaction service. (Marius Preda)
    -   Added functionality to add and view children's activities (meal, sleep, behavior). (Marius Preda)
    -   Added MongoDB for operational data storage. (Marius Preda)
    -   Integrated mongo-express for database management. (Marius Preda)
    -   Added proper testing and route fixes (Marius Preda)
-   **Activity Log Service:**
    -   First version of activity log implementation. (Alexandra Burnichi)
    -   Added a basic readme. (Marius Preda)
-   **Child Profile Service:**
    -   First version of child profile implementation. (Alexandra Burnichi)
    -    Added first version of the child profile implementation (Alexandra Burnichi)
### Changed
-   **Auth Service:**
    -   Minor readme change (Marius Preda)
    -   Readme improvement (Marius Preda)
    -   Comment changes (Marius Preda)

### Removed
-   **Auth Service**:
    -   Deleted placeholder secrets files (Marius Preda)

## [0.9.0] - 2025-04-20
### Added
-   Initial commit for several services:
    -   Auth Service: Basic authentication implementation. (Marius Preda)
    -   DB Interact Service: Initial commit. (Marius Preda)
    -   Activity Log Service: Initial commit. (Alexandra Burnichi)
    -   Child Profile Service: Initial commit. (Alexandra Burnichi)
