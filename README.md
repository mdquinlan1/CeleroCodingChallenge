# CeleroCodingChallenge
A coding challenge for CeleroCommerce as part of the interview.

### Creator Info
    Matthew Quinlan
    11/1/2020
---

### Overview
  ## Purpose
  - The purpose of this application is to allow technicians to see information about the tasks they need to perform for certain clients.
      - This information includes: location (address) of the client, issue to be resolved, pictures of the issue, etc.
  ---
  ## Approach
  - The approach I took while developing this app was attempting to follow MVVM Architecture principles and maintaining separation of concerns. This was most-likely why I was unable to finish the requirements as I spent most of my time figuring out how to structure the application with low coupling and high cohesion.
  - The list of clients is shown as containers in a recyclerview
  - The application is set up to easily allow implementation of json parsing by using the repository to extract the json (using most likely gson and retrofit), and then storing that parsed information into the database (ROOM). This allows the persistence of data (while internet is unavailable). Should the json on the server be updated or modified while the device has no access to the server (internet unavailable), once internet is restored, the repository will parse the data and update the table in the database.
  - The viewmodel has access to the database and can then display the data in an easy to read fashion.
  ---
---

---


