hdp-ranger-deploy-certs
=========

Deploys certificates for ranger ssl from a defined directory and adds them to their corresponding keystores and
truststores as defined in the ranger-policy-manager-ssl.xml

Requirements
------------

Certificates must be available in the ssl_certs directory by putting them
there manually or running the hdp-create-ranger-certs role using the same
config file first.

Role Variables
--------------


Dependencies
------------

hdp-ranger-create-certs

Example Playbook
----------------

    - hosts: hbase
      roles:
         - { role: hdp-ranger-deploy-certs, service: hbase }

License
-------

BSD

Author Information
------------------

Stefan Kupstaitis-Dunkler (stefan.dun@gmail.com)
