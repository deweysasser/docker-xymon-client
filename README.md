docker-xymon-client
===================

A dockerized [xymon](http://xymon.sourceforge.net/) client to monitor
any host


Usage
-----

```
docker run -d --net=host --name xymon-client -e XYMONSERVERS="xymon.example.com" deweysasser/xymon-client
```

where 'xymon.example.com' is the name of your xymon server.

If you'd like to monitor disk space on anything other than
/var/lib/docker, you should mount a volume in the appopriate file
system into the container somewhere.  Location is irrelevant.


See Also
--------

See also the containerized [Xymon server](https://hub.docker.com/r/deweysasser/xymon/).