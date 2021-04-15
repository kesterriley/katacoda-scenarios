# Repository Files

MariaDB provides a simple-to-use script to install the repository files to your server.

When you run this script it will install a repository file to tell `yum` where to look for the RPM files to install.

It is possible to specify the version of MariaDB that you would like installed. This can be set with the `mariadb-server-version` parameter.

`curl -sS https://downloads.mariadb.com/MariaDB/mariadb_repo_setup | bash -s -- --mariadb-server-version=mariadb-10.3`{{execute}}

Once you have run the command you can check that the file is installed.

`cat /etc/yum.repos.d/mariadb.repo`{{execute}}

