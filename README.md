CouchDB Google Storage Backup
=============================

CouchDB Google Storage Backup Role for Kazoo Ansible

Requirements
------------

None

Role Variables
--------------

User Variables
- couchdb_google_storage_backup_bucket_name - The Google Cloud 
  Storage Bucket to upload backups to
- couchdb_google_storage_backup_service_account_key: - The 
  contents of the Google Cloud Service Account credentials.json 
  to use for authentication

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: kazoo-ansible.couchdb-google-storage-backup,
             couchdb_google_storage_backup_bucket_name: couchdbbackup,
             couchdb_google_storage_backup_service_account_key: 
             contents of credentials.json }

License
-------

MIT

