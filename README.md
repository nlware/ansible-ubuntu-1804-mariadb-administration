## ubuntu-1804-mariadb-administration

Administer databases and users on MariaDB server in Ubuntu 18.04.

#### Variables

* `ubuntu_1804_mariadb_administration_databases_present`: [default: `{}`]: Databases to create
* `ubuntu_1804_mariadb_administration_databases_present.{n}.name`: [required]: The name of the database
* `ubuntu_1804_mariadb_administration_databases_present.{n}.collation`: [optional, default: `utf8mb4_general_ci`]: The collation of the database
* `ubuntu_1804_mariadb_administration_databases_present.{n}.encoding`: [optional, default: `utf8mb4`]: The character set of the database

* `ubuntu_1804_mariadb_administration_databases_absent`: [default: `[]`]: Databases to drop

* `ubuntu_1804_mariadb_administration_users_present`: [default: `[]`]: Users to create
* `ubuntu_1804_mariadb_administration_users_present.{n}.name`: [required]: The name of the user
* `ubuntu_1804_mariadb_administration_users_present.{n}.password`: [required]: The password of the user
* `ubuntu_1804_mariadb_administration_users_present.{n}.priv`: [optional, default: `name + '.*:ALL'`]: Privileges
* `ubuntu_1804_mariadb_administration_users_present.{n}.host`: [optional, default: `localhost`]: Host to create privileges for

* `ubuntu_1804_mariadb_administration_users_absent`: [default: `[]`]: Users to drop
* `ubuntu_1804_mariadb_administration_users_absent.{n}.name`: [required]: The name of the user
* `ubuntu_1804_mariadb_administration_users_absent.{n}.host`: [optional, default: `localhost`]: Host to drop privileges for
