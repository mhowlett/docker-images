### Docker Cheat Sheet

Misc notes on how to make docker do stuff.

#### boot2docker

##### temporary port forwarding:

boot2docker ssh -vnNTL 8000:localhost:8000

more notes on that here:

https://github.com/boot2docker/boot2docker/blob/master/doc/WORKAROUNDS.md

##### initializing env

$(boot2docker shellinit)
