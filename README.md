# GPing #
This is a fork of gping project, things currently changed is for reducing the CPU spikes by reducing the context switching of timeout grrenlet and other minor things. For some reason, die was not working, it wwas worked up to make it work. Some more changes might come in future as I test it further in production.

This is a fork of the python-ping project that strips out most everything and replaces it with gevent. The point is to have an event driven ping utility for doing many concurrent pings...

## Example Usage ##

    gp = GPing()
    gp.send("127.0.0.1",test_callback)
    gp.join()
    gp.die()

## Install ##

This *should* be easy on your average \*nix box (raw sockets are needed). Just type `sudo pip install gping`

## License and Credits ##

The python-ping project was started by Matthew Dixon Cowles.

	- copyleft 1989-2011 by the python-ping team, see AUTHORS for more details.
	- license: GNU GPL v2, see LICENSE for more details.

I have left the license and authors information intact, but this project seems to have a long history or forks and such so I am probably somehow pissing someone off or violating some license. Let me know if this is the case and I will be better. 
