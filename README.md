# deepplantphenomics-PlantIT

This repo is used to serve as a flow on [PlantIT](http://portnoy.cyverse.org/) that can conduct the semantic section pre-trained model on [IPPN dataset](https://www.plant-phenotyping.org/datasets-home).

Deep plant phenomics is a python package developed and [published by Ubbens and Stavness](https://www.frontiersin.org/articles/10.3389/fpls.2017.01190/full).

A truncated version of deepplantphenomics python package is in the other_module dir for the usage of docker image building recipe.

## to do list
[] check how to correctly save the output
[] build singularity image
[] prepare other scripts

## semantic section example USAGE
* Any image in the specified dir with suffix '_rgb.png' can be read in the model.
* Use -p to specify the input path dir. The -ft will be removed.
* Local testing command (script correctly run but cannot obtain output files):
```
docker run -v /path/to/image/:/home/ docker://bendjamin101001/plantit_dpp:v1 python3 semantic_section_example.py -p /home/ -ft jpg
```
