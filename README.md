This is a Dockerfile for [Mitsuba2](https://github.com/mitsuba-renderer/mitsuba2).

Build:
```
$ docker build -t mitsuba2-docker .
```

Run:
```
$ docker run -it mitsuba2-docker bash
```

# Choosing variants
You can change this setting by editing `mitsuba.conf.cpu`.

The current setup enables:
```
    "scalar_rgb",
    "scalar_spectral",
    "scalar_rgb_polarized",
    "scalar_spectral_polarized",
    "packet_rgb",
    "packet_spectral"
```

Note that this dockerfile does not support GPU dependency.