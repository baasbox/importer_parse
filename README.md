importer_parse
==============

####The configuration files for the ETL process from Parse to BaasBox

Please follow this [link] https://github.com/orientechnologies/orientdb-etl/wiki for the Installation and Usage guide 

At the moment the ETL process from Parse to BaasBox for users is available only partially  
**check at the end of this file for the issues**

First of all, save the backup of the Parse user in a JSON (i.e. Users-parse.json)
Now write the exact path of the file .json at the section source for every configuration file

Like in this example
"source" : {
"file": { "
path": "/Users/user/databases/parse/User-backup-parse.json", "lock" : true }
  }
  
At the loader section, please insert the right credentials and the path for BaasBox db.
(The default credentials are admin for username and admin for password)

Please note that there are some issues for users' ETL, so the ETL process for users is **incomplete**
