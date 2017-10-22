## ubuntu-1604-mariadb-administration

Administer databases and users on MariaDB server in Ubuntu 16.04.

#### Variables

* `ubuntu_1604_mariadb_administration_databases_present`: [default: `[]`]: Databases to create

* `ubuntu_1604_mariadb_administration_databases_absent`: [default: `[]`]: Databases to drop

* `ubuntu_1604_mariadb_administration_users_present`: [default: `[]`]: Users to create
* `ubuntu_1604_mariadb_administration_users_present.{n}.name`: [required]: The name of the user
* `ubuntu_1604_mariadb_administration_users_present.{n}.password`: [required]: The password of the user
* `ubuntu_1604_mariadb_administration_users_present.{n}.priv`: [optional, default: `name + '.*:ALL'`]: Privileges
* `ubuntu_1604_mariadb_administration_users_present.{n}.host`: [optional, default: `localhost`]: Host to create privileges for

* `ubuntu_1604_mariadb_administration_users_absent`: [default: `[]`]: Users to drop
* `ubuntu_1604_mariadb_administration_users_absent.{n}.name`: [required]: The name of the user
* `ubuntu_1604_mariadb_administration_users_absent.{n}.host`: [optional, default: `localhost`]: Host to drop privileges for
