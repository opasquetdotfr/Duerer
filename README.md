# Duerer

![TOI-1842_b_zoom_2](./img/TOI-1842_b_zoom_2.jpg)

Audio synthesis and virtual acoustics for [Rhino](https://www.rhino3d.com) [Grasshooper](https://www.rhino3d.com/6/new/grasshopper/) based on image source model room simulation.\
For future more information see [here](https://www.opasquet.fr/spatial-computing-composition/).\
This release consists on python code runing underneath and collection of [Grasshooper](https://www.rhino3d.com/6/new/grasshopper/).

This is an early experimental version.

*Duerer* is part of a research done at the Institute for [Institute for Computer Music and Sound Technology](https://www.zhdk.ch/en/research/icst) of the [Zurich University of the Arts Zurich University of the Arts](https://www.zhdk.ch).

The first use would consist on:
- generating, or importing, a tree of meshes.
- setting meshes acoustic properties and redering parameters (those do not have to be realistic and outcomes can be used as a virtual acoustic or synthesis tool).
- place virtual sources and microphones into those meshes.
- (define directivities for sources and microphones).
- define sound sources.
- rendering as a multichannel [Impulse response](https://en.wikipedia.org/wiki/Impulse_response) file (each channel is a microphone) and possibly a convolved file made with sound sources.

One possible use would consist on rendering multichannel impulse responses from a beam of microphones or a virtual eigenmike; thus playing with directivity, delays and virtual [ambisonics](https://en.wikipedia.org/wiki/Ambisonics).\
Another use would be using specific meshes to generate physical models audio synthesis from finite elements method.\
I also used for form finding using genetic algorithm solvers like [galapagos](http://climatefacade.com/genetic-algorithm-solver-galapagos/) for instance.


## Technologies Used
- [Rhino](https://www.rhino3d.com)
- [Grasshooper](https://www.rhino3d.com/6/new/grasshopper/)
- [Pyroomacoustics](https://pyroomacoustics.readthedocs.io)


## Screenshots
Available Grasshooper components:\
![Available Grasshooper components](./img/Renderer.png)

Components dealing with spectral absorption for each mesh face:\
<center><img src="https://github.com/opasquetdotfr/Duerer/blob/5de80a9b58fbd3efe37252ab51d34eeb8fc3719c/img/Material_1.png" width=50% height=50%></center>


## Project Status
Project is: _in progress_
<!--/ _complete_ / _no longer being worked on_. If you are no longer working on it, provide reasons why.-->


## Dependencies
  ```shell
rhino3d
pyroomacoustics
numpy
scipy>=0.18.0
cython
pybind11
  ```

## Acknowledgements
- Many thanks to Jasch, Toro-Pérez Germán for their support and Robin Scheibler for his tremendous work on Pyroomacoustics. I would have never done that work without the support of the [Zurich University of the Arts Zurich University of the Arts](https://www.zhdk.ch).


## Contact
Created by [Olivier Pasquet](https://www.opasquet.fr).
