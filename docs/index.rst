============
Messidge RPC
============

**Messidge is a message passing framework for distributed systems needing a public gateway.**

Messidge is a Python 3 client server rpc with a few differences: It enforces public/private encryption, and is able to guarantee the provenance of a particular message; synchronous, asynchronous and streaming replies are trivial; and are all multiplexed over a single connection.

Having a background in `containers <https://20ft.nz/>`_, Messidge also has a concept of nodes - being services provided across a private LAN (or VPC) that can be announced as part of a resource offer when the client connects. There are no 'addresses' as such and these services are provided transparently as if they are part of the server.

The details...

* User connections are through asymmetric keys (via libnacl).
* Includes a lightweight invite/confirm server for client accounts.
* Handles session management for client connections.
* Automatic fail/reconnect with event callbacks.
* Tolerant of slow block devices.
* ZeroMQ, cbor and multiprocessed encryption.

Above all it's simple, fast, and well suited to agile development.

----

..  toctree::
    :maxdepth: 2
    :caption: Contents:

    quickstart
    use
    administer
    ref
