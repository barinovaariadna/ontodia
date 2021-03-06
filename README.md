# Ontodia #

Ontodia is a JavaScript library that allows to visualize, navigate and explore the data in the form of an interactive graph based on underlying data sources. The library is a major front-end component in <a href="http://ontodia.org">ontodia.org</a> web application that provides semantic data visualization services.

### What is Ontodia for? ###

Ontodia is a JavaScript library that allows you to create and persist diagrams made from data - relational, object, semantic.

It was designed to visualize RDF data sets in particular, but could be tailored to almost any data sourece by implementing data provider interface.  

### How do I get set up? ###

#### Quickly get up and running ####

You can get Ontodia from npm repository: `npm install ontodia`
 
To quickly get Ontodia up and running you can run `npm install && npm run demo`, it will compile everything, output connection string for you browser in the console and you can start trying it.

* [http://localhost:10444/](http://localhost:10444/) will display Ontodia with static build-in data.
* [http://localhost:10444/sparql.html](http://localhost:10444/sparql.html) will display Ontodia with SPARQL endpoint set in `SPARQL_ENDPOINT` environment variable.

The actual port could vary in your case, please see output of `npm run demo` for correct port.

#### Usage of TypeScript ####

Ontodia library heavily uses TypeScript language. All type definitions are exported along with a library. It's not required to use TypeScript to use this library, but even for JS developers it's worth through TypeScript sources or ontodia.d.ts build output file to know API.   

#### Usage of library in you own code ####

Ontodia interface is React-based application and you should initialize React component to work with. You can see example of initializing library in src/examples/template.ejs and /home/yuricus/projects/ontodia/src/examples/demo.ts

#### API ###
You can:

- get diagram layout
- initialize ontodia with stored layout
- specify you own action for clicking on element's URIs

#### Building Ontodia ####

You could build Ontodia from source with `npm install && npm run build`

#### Licence ####

Ontodia library is distributed under LGPL-2.1

#### Dependencies ####

- d3 - used to create element interface
- intro.js - used to display overlay help
- jointjs - diagramming library Ontodia builds upon
- jquery - dependency of jointjs
- lodash - general purpose utility library
- n3 - library to parse SPARQL endpoint responses.
- springy - force directed layout implementation

### Contribution guidelines ###

- Please create pull request describing changes 
- Please follow STYLEGUIDE

### Who do I talk to? ###

Feel free to write to ontodia-people@vismart.biz
