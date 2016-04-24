mjpg-streamer output plugin: output_simplehttp
========================================

This plugin streams JPEG data from input plugins via HTTP (simplified).
Basically this is the same as output_http but with all extra functionality
stripped. Only mjpg stream and snapshots are supported.

Usage
=====

    mjpg_streamer [input plugin options] -o 'output_simplehttp.so [options]'

```
---------------------------------------------------------------
The following parameters can be passed to this plugin:

[-p | --port ]..........: TCP port for this HTTP server
[-c | --credentials ]...: ask for "username:password" on connect
---------------------------------------------------------------
```

Browser/VLC
-----------

To view the stream use VLC or Firefox/Chrome and open the URL:

    http://127.0.0.1:8080/stream

If there are multiple input plugins, you can access each stream individually:

    http://127.0.0.1:8080/stream0
    http://127.0.0.1:8080/stream1

To view a single JPEG just open this URL:

    http://127.0.0.1:8080/snapshot

