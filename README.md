stool
=====

like a couchapp, only with a euphamistic name.

To create a database, run ./stool -n <db-name> -s <db-host-server> -d <ddocs>
Where <ddocs> points to a directory in which all design documents are held.  Each design document should be a new sub-directory, with each document parameter (e.g. views) a sub-directory of this.  For example:

Two design documents will be created, one is called D1, the other D2.  These are held in the folder:

/home/user1/NewCouchDB

D1 contains two views, each with a map and reduce function, called V1 and V2.  The directory structure would be:

/home/user1/NewCouchDB/D1
/home/user1/NewCouchDB/D1/views
/home/user1/NewCouchDB/D1/views/V1
/home/user1/NewCouchDB/D1/views/V1/map.js
/home/user1/NewCouchDB/D1/views/V1/reduce.js
/home/user1/NewCouchDB/D1/views/V2
/home/user1/NewCouchDB/D1/views/V2/map.js
/home/user1/NewCouchDB/D1/views/V2/reduce.js

D2, meanwhile, contains one view (V1) but also has some attachements (index.html and a css folder with styles.css):

/home/user1/NewCouchDB/D2
/home/user1/NewCouchDB/D2/views
/home/user1/NewCouchDB/D2/views/V1
/home/user1/NewCouchDB/D2/views/V1/map.js
/home/user1/NewCouchDB/D2/views/V1/reduce.js
/home/user1/NewCouchDB/D2/attachments
/home/user1/NewCouchDB/D2/attachments/index.html
/home/user1/NewCouchDB/D2/attachments/css
/home/user1/NewCouchDB/D2/attachments/css/styles.css
