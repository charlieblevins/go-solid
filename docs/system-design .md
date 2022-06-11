# System Design 

## WebID

### Expected Operations
- check that id exists
- get metadata by id (like root directory ID)
- 

## Non-RDF Files

### Expected Operations
- get file contents by path
- set file contents by path

### Solutions
- S3 bucket named with users web id
- bucket contains no directories - flat listing
- lookup s3 id in dynamo table indexed by file path

## RDF Files

### Expected Operations
- get triples in file 
- create/update/delete triple in file

### Solutions
- dynamo table called "rdf-triples", indexed by file path. holds path, noun, relation, direct-object

## Folders

### Expected Operations
- get folder contents by folder path 
- get parent folder by folder path
- delete all contents in folder and sub-folders ???
- more? check spec/NSS for all endpoints

### Solutions
- neo4j?

## Other Notes
- all indexed fields in dynamo must be prefixed with user's id (webid in some form)
