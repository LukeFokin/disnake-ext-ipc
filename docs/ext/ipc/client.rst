Client Connection
=================

The IPC client is very simple.
It will simply connect to your server process and send JSON data.
If you do not supply a port on initialisation, the client will connect to the multicast :doc:`server<server>` and return the port from said server.

If you do supply a port, it will connect to the server instantly.

Requests are made by calling :py:meth:`Client.request`
and will be sent to the server in the json format specified above.
It will then wait for a response and return the data.

.. currentmodule:: disnake.ext.ipc.client

.. autoclass:: Client
    :members:
