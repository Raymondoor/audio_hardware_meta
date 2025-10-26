# Audio Hardware Metadata Collection

I wanted to create an easy way to organize audio equipment, such as Audio interfaces and Mixers.

- Overall/Global data
    - Stuff like dimensions and vendors goes here.
- Ports (p):
    - All the I/O information of signals comes here. Physical shapes, Supported signal type, and so on.
- Process (x):
    - This is internals that is not exposed to external I/O. Gain, Effects, Monitoring modes, mix/splits, and so on comes here. Partially implemented.
- Controls (c):
    - This is where all the user controlled components gets defined. Things like faders, knobs and buttons come here. This itself only should hold values of how the value will change, not the value itself. [Continuous, Discrete, Boolean]
- Routing:
    - This is for the internals that connect Ports/Process/Controls A to Ports/Process/Controls B. Should be just {"from": "xx", "to": "xx"}. A routing does not connect to another routing, must have any of the obove in between. Partially implemented.
- Meta:
    - Some general organizing of data that is useful to humans. Such as stereo. Modern software can do many things and it may not be able to cover the entire "settings" each equipment has. Perhaps this is for that. Partially implemented.

This project is useful by itself, but is intended for another of my personal's, I wanted to make a tool for creating diagrams for my audio hardware setup.

The goal of this repo is to make a good enough data schema for the devices, and to actually populate the data somewhere, in a database. So help me if you want to :)

This is not a complete project, an unstable commit may be pushed.