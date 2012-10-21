sqlbench
=============

Benchmark MySQL databases

Usage
-----

	sqlbench [-H <host>] [-P <port>] [-u <user>] [-p <password>] [-d <db>]
			[-C <charset>] [-w <workers>] [-c <conc>] [-o <log>]
			<sql list file>

where

	-H <host>		Specifies database host. Default to "localhost"
	-P <port>		Specifies database port. Default to 3306
	-u <user>		Specifies user name. Default to "root"
	-p <password>	Specifies password. Default to ""
	-d <db>			Specifies database name. Default to "test"
	-w <workers>	Specifies number of worker processes. Default to 0 (auto)
	-c <conc>		Specifies concurrent connections per worker. Default to 10
	-o <log path>	Specifies timing log path. Default to "result.log"
	<sql list file>	Specifies file with testing SQLs list (newline separated)

Note: SQL statements in the list file must be in UTF-8 encoding!

Dependency
----------

* node
* npm install optimist mysql line-reader

Author
------

Xiaozhe Wang <chaoslawful [at] gmail.com>

