teamspeak_server controller
================

Basic controller for a teamspeak_server

This controller responds to actions defined in the teamspeak server metadata file:

* Decom -  deletes local and remote datastores (sqlite/mysql), and deletes log files

Note: this controller does not yet support deleting remote mysql dbs

To use the controller start it with the required arguments for your command, and
the mounted volumes from the associated container

```
docker run --rm --volumes-from my_teamspeak_server bfosberry/teamspeak_controller decom
```
 
