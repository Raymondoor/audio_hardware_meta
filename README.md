# Audio Hardware Metadata Collection

I wanted to create an easy way to organize audio equipment, such as Audio interfaces and Mixers.

- Overall/Global data
    - Stuff like dimensions and vendors goes here.
- Port:
    - All the I/O information comes here. Physical shapes, Supported signal type, and so on.
- Patch:
    - This is internals that is not exposed to external I/O. Gain, Effects, Monitoring modes comes here. Have not implemented yet.
- Routing:
    - This is for the internals that connect Port/Patch A to Port/Patch B. Have not implemented yet.
- Meta:
    - Some general organizing of data that is useful to humans. Such as stereo. Modern software can do many things and it may not be able to cover the entire "settings" each equipment has. Perhaps this is for that. Have not implemented yet.

This project is useful by itself, but is intended for another of my personal's, I wanted to make a tool for creating diagrams for my audio hardware setup.

The goal of this repo is to make a good enough data schema for the devices, and to actually populate the data somewhere, in a database. So help me if you want to :)