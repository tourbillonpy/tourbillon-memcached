Configure
*********


Create the tourbillon-memcached configuration file
==============================================

You must create the tourbillon-memcached configuration file in order to use tourbillon-memcached.
By default, the configuration file must be placed in **/etc/tourbillon/conf.d** and its name
must be **memcached.conf**.

The tourbillon-memcached configuration file looks like: ::

	{
		"database": {
			"name": "memcached",
			"duration": "365d",
			"replication": "1"
		},
		"hostname": "localhost",
		"port": 11211,
		"frequency": 1
	}


You can customize the database name, the retencion policy and the memcached connection parameters.


Enable the tourbillon-memcached metrics collectors
==================================================

To enable the tourbillon-memcached metrics collectors types the following command: ::

	$ sudo -i tourbillon enable tourbillon.memcached=get_memcached_stats
