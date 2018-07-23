# mongo-db
Automated Bash MongoDB 3.2.X Install Script for Debian/ Ubuntu

The following is a brief outline of the steps the script takes:

1. Add the apt repository from mongodb.org and associated key.
2. Install the full mongo-org package containing these packages: mongodb-org-server, mongodb-org-mongos, mongodb-org-shell, mongodb-org-tools.
3. Add a basic config file that:
      Enforces the wiredTiger storage engine.
      Enables remote access by listening on ALL interfaces.
      Enables replication, even if it’s just a stand alone node.
      Enables user authentication.
4. Initiates the server as a replication cluster.
5. Adds a user for administration called admin with password admin.
