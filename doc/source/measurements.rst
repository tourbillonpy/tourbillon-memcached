Measurements
************

tourbillon-memcached collects metrics about the cache.

Please refers to  `https://github.com/memcached/memcached/blob/master/doc/protocol.txt <https://github.com/memcached/memcached/blob/master/doc/protocol.txt>`_ for more information.


Memcached stats
===============

tourbillon-memcached store metrics in the ``memcached_stats`` series.
Each datapoint is tagged with the memcached instance hostname and the values collected are:


Tags
----
	* **host**: memcached instance hostname

Fields
------

The collected fields depends on the Memcached version.

In the following list there are the fields collected if they exist.

    * connection_structures
    * incr_misses
    * conn_yields
    * listen_disabled_num
    * cas_misses
    * rusage_system
    * bytes 
    * delete_hits
    * hash_bytes
    * reserved_fds
    * curr_items
    * pointer_size
    * cmd_flush
    * cas_hits
    * threads
    * bytes_read
    * evictions
    * reclaimed
    * curr_connections
    * accepting_conns
    * get_misses
    * total_connections
    * incr_hits
    * cmd_touch
    * decr_misses
    * get_hits
    * bytes_written
    * rusage_user
    * auth_cmds
    * decr_hits
    * hash_power_level
    * hash_is_expanding
    * cmd_set
    * cas_badval
    * cmd_get
    * delete_misses
    * limit_maxbytes
    * touch_misses
    * total_items
    * evicted_unfetched
    * touch_hits
    * expired_unfetched
    * auth_errors
