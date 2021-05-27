# helio-flyway

This repo uses Flyway Migration tool: https://flywaydb.org/ which will migrate and version the database to the current
needed state.

### Usage
To run either run the `build` and `flywayMigrate` commands, after setting the build.gradle URL/user/password fields

OR

Run the command via gradlew shell script or gradlew.bat by passing in the variables (or build.gradle)

E.g., 

`gradlew -Pflyway.user=postgres -Pflyway.url=jdbc:postgresql://<url>/<database> -Pflyway.password=<password> flywayMigrate`

# Part 1 Challenge Tasks:
1. Pick 2 files from the src/main/resources/files directory (other than Acronyms) that have some similar properties 
   (e.g. drug name, state, etc.)
2. Create 2 Tables for both files and add the table creations to the migrations steps. Consider your table design please.
3. Load the data into their respective tables
    - Data can either be loaded via migration script, or some call/function via Flyway 
      (language choice does not matter here as long as it runs within this project via `flywayMigrate`)
    
Note: if loading via migration script, how you generate it does not need to be included, as could be a tool/IDE or a 
program if you so choose. As long as we have a valid migration script, or any way to load the data that `flywayMigrate` 
can initiate, this step will be satisfied for the purpose of this challenge.
