Tonewheel Organ
===============

A virtual tonewheel organ and emulated rotary speaker in PureData.

You may be more familiar with the trade names, Hammond Organ and Leslie Speaker; these are the famous makers of these instruments.

Features
--------

The organ consists of 8-voice polyphony (though this is easily extendable to any number of voices), and drawbar emulation. The rotary speaker is simulated with stereo panning.

Running
-------

You must have an installation of `PureData <https://puredata.info>`_ to use this instrument. For the rotary speaker to work, you need to have a stereo output, sometimes laptops don't have this.

``hamwrap.pd`` is the main patch to open. The abstractions ``hammond~.pd`` and ``leslie~.pd`` are the implementations of the organ and rotary speaker.

It is highly recommended to have a low latency audio subsystem. On Linux the most common solution is `JACK <jackaudio.org>`_, but JACK is also available for OSX and Windows. macOS users will probably be fine with the default CoreAudio drivers. Windows users will almost certainly want to try ASIO or JACK.

License
-------

Licensed under GPLv3
