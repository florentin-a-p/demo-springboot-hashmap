# demo-springboot-hashmap

A Java Springboot application that provides CRUD APIs that can read and update countries, which are stored in HashMap. The build tool is Gradle. The next iteration will store the countries in a database https://github.com/florentin-a-p/demo-springboot-database


| **Description**     | **Request**                                                                                                                                       | **Expected Response** |
|---------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| get all countries   | curl http://localhost:8080/getCountries                                                                                                           |                       |
| get country by id   | curl http://localhost:8080/getCountries/2                                                                                                         |                       |
| delete country      | curl -X DELETE  http://localhost:8080/deleteCountry/1                                                                                             |                       |
| update country      | curl -X PUT -d '{"id":2,"countryName":"Japan","countryCapital":"Tokyo"}' -H "Content-Type: application/json"  http://localhost:8080/updateCountry |                       |
| get country by name | curl http://localhost:8080/getCountries/countryName?name=India                                                                                    |                       |
| add new country     | curl -X POST -d '{"countryName":"Italy","capital":"Rome"}' -H "Content-Type: application/json"  http://localhost:8080/addCountry                  |                       |
