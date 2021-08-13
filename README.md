Burrito Overlay
===============
Burrito is an early alpha overlay tool for Guildwars 2 that runs on linux without any display hacks.

The primary goal is to render and edit POIs and routes based off of sharable data files while being able to run on linux with no workarounds.

It functions natively linux via running a pre-compiled binary inside of wine that streams the memory mapped data back to the host.


Getting Started
===============
Go to [burrito.orthogonalprojects.com](https://burrito.orthogonalprojects.com) for instructions


Roadmap
=======
* Automatically run the burrito_link binary when burrito starts.
* Launch the burrito_link binary via an internal config instead of via an external script.
  * A seperate script to generate the config from Lutris settings automatically.
* Automatically close burrito when GW2 closes.
* Automatically parse/convert TacO marker files instead of using a converter script.


Known Bug Workarounds
=====================
* Burrito launches off-center or on the wrong monitor
  * This seems to be WM dependant. on Gnome it can be solved by holding down the super key and dragging burrito to the right position.
* Burrito does not allocate space for the mumble mmap
  * This can be fixed by running some other program that takes advantage of the link such as arcdps.
