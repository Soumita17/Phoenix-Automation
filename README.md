## Phoenix Automation for InWarranty QC Accept using Postman

### API endpoint: GET http://phoenix.techwithjatin.com

### **Author**: Soumita

## Project Overview

Phoenix Automation is a collection of Postman API requests used for testing the functionalities of the Phoenix platform. The automation is integrated with Newman for CLI execution, along with `newman-reporter-html-extra` for enhanced reporting. The environment file used for testing is `QA.postman_environment.json`, and the tests are set up for continuous integration using GitHub Actions.

## Techstack
1. Postman API
2. Node.js
3. Newman
4. Gitbas
   
## Prerequisites

1. **Postman**: Make sure Postman is installed to work with the collection.
2. **Newman**: Install Newman globally to run the collection from the command line.
    ```bash
    npm install -g newman
    ```
3. **Newman HTML Extra Reporter**: Install the HTML reporter for enhanced report generation.
    ```bash
    npm install -g newman-reporter-html-extra
    ```

## Running the Collection

To execute the collection in your terminal using Newman, follow these steps:

1. Clone the repository and navigate to the project directory.
2. Use the following command to run the Postman collection with the `QA` environment:
   ```bash
   newman run Inwarranty\ QC\ Accept.postman_collection.json -e QA.postman_environment.json -r html-extra
