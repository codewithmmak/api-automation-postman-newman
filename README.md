# Automating OData based RESTful API using POSTMAN

## How to run Postman Collection using Postman tool?
1. Open Runner
2. Drag and Drop your collection
3. Select the tests
4. Hit Run button
![Automating OData based RESTful API using POSTMAN](./img/postman-result.png?raw=true "Automating OData based RESTful API using POSTMAN Test Results")

## How to run Postman Collection using Newman CLI tool?
1. Open Terminal/CMD
2. Install newman `npm install -g newman`
3. Go to root path of project
4. Enter command
`newman run OData_In_6_Steps.postman_collection.json`
5. CLI will show below results

![Automating OData based RESTful API using POSTMAN](./img/cli-result-01.png?raw=true "Automating OData based RESTful API using POSTMAN Test Results")

![Automating OData based RESTful API using POSTMAN](./img/cli-result-02.png?raw=true "Automating OData based RESTful API using POSTMAN Test Results")

## How to generate HTML report using npm newman-reporter-html with Newman?
1. Open Terminal/CMD
2. Install reporters `npm install -g newman-reporter-html`
3. Go to root path of project
4. Enter command
`newman run OData_In_6_Steps.postman_collection.json -r html`

## How to generate HTML report using npm newman-reporter-htmlextra with Newman?
1. Open Terminal/CMD
2. Install reporters `npm install -g newman-reporter-htmlextra`
3. Go to root path of project
4. Enter command
`newman run OData_In_6_Steps.postman_collection.json -r htmlextra --reporter-htmlextra-export .\testResults\TestResult.html`

![Automating OData based RESTful API using POSTMAN](./img/htmlextra-result.png?raw=true "Automating OData based RESTful API using POSTMAN Test Results")

## How to generate CSV report using npm newman-reporter-csv with Newman?
1. Open Terminal/CMD
2. Install reporters `npm install -g newman-reporter-csv`
3. Go to root path of project
4. Enter command
`newman run OData_In_6_Steps.postman_collection.json -r csv --reporter-csv-export .\testResults\TestResult.csv`

![Automating OData based RESTful API using POSTMAN](./img/csv-result.png?raw=true "Automating OData based RESTful API using POSTMAN Test Results")

## Troubleshooting
Issue #1: When you run Postman collection using newman you may see error: 
File C:\Users\admin\AppData\Roaming\npm\newman.ps1 cannot be loaded because running scripts is disabled on this system. For more information, see about_Execution_Policies at https:/go.microsoft.com/fwlink/?LinkID=135170.
Solution: Follow step 1 to 3 given on `https://www.c-sharpcorner.com/article/how-to-fix-ps1-can-not-be-loaded-because-running-scripts-is-disabled-on-this-sys/`