# helio-flyway

This repo uses Flyway Migration tool: https://flywaydb.org/ which will migrate and version the database to the current
needed state.

### Usage
To run either run the `build` and `flywayMigrate` commands, after setting the build.gradle URL/user/password fields

OR

Run the command via gradlew shell script or gradlew.bat by passing in the variables (or build.gradle)

E.g., 

`gradlew -Pflyway.user=postgres -Pflyway.url=jdbc:postgresql://<url>/<database> -Pflyway.password=<password> flywayMigrate`
