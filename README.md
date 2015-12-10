Role Name
=========

Role for loading test data (or, maybe, other data) to a preference server data stores (CouchDB instance). Split out from ansible-preferences-server.

Requirements
------------

* Running couchdb server to load the data to.

Role Variables
--------------

preferences_server_data_loader_couchdb_host_address: couchdb (default - localhost:5984)
preferences_server_data_loader_cleanup_after: whether or not to delete kanso and the temporary directory (default - true)
preferences_server_data_loader_clear_index: should we clear the /preferences index in couchdb and create it again? (default - true)

Dependencies
------------

* [ansible-facts](https://github.com/idi-ops/ansible-facts) role
* [ansible-nodejs](https://github.com/idi-ops/ansible-nodejs) role, since it checks out universal and needs to install Kanso

Example Playbook
----------------


License
-------

MIT

Author Information
------------------
