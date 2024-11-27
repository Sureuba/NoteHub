# Back End Development and APIs NOTES
### FreeCodeCamp.com

Learning: **Javascript** for backend, 
**Node.js** (framework) and **npm** (package manager)

**Express** (framework), **MongoDB** and Mongoose library

### Managing Packages with NPM

npm (Node Package Manager), is a command line tool to install, create, and share packages of JavaScript code written for Node.js. There are many open source packages available on npm, so before starting a project, take some time to explore so you don't end up recreating the wheel for things like working with dates or fetching data from an API.

**package.json - What does it do** 
* Stores info on the project, has a single JSON object. 
* Information is stored in Key-Value pairs.
* Stores metadata.
* 2 required fields: name, version

**Creating a package.json** 

Command: npm init -y (-y will generate the file without questions)

**Adding fields in the Package.json file**<Br/>
author field: specifies who created the project, string or object with contact detail, etc.

Ex: "author" : "Jane Doe"
"description": "What this project does"

Keywords: describe project with related keywords
