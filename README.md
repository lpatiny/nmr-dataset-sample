https://deploy-preview-106--nmrium-org.netlify.app/teaching#?toc=https://cheminfo.github.io/nmr-dataset-sample/toc.json

https://deploy-preview-106--nmrium-org.netlify.app/teaching#?toc=https://cheminfo.github.io/nmr-dataset-sample/toc.json

## NMRium for teaching

It is possible to use www.nmrium.org to teach NMR structural elucidation.

## Creating your own series

You should first clone this project

You may then change all the files and folder. You have the possibility to group exercises in folder or have them directly at the first level.

## NMR spectra format

You should save the NMR spectra as a JCAMP-DX file (on topspin use the `tojdx` command). The spectrum should be FT and phase corrected. To spare bandwidth you may only save the real part of the spectrum.

## One folder = One exercise

For each exercise you want to create you should can add the following files:

- structure.mol : mandatory, the chemical structure of the answer
- 1h.jdx
- 13c.jdx
- 13cdec.jdx
- cosy.jdx
- hsqc.jdx
- hmbc.jdx
- deptXXX.jdx
- aptXXX.jdx
- ...

Only folder that contain an answer (`structure.mol`) will be processed.

## Building the toc

The system is based on various JSON files that are build automatically. In order to build the `toc.json` you first need to install [node.js](https://nodejs.org/).

You should then install our `nmrium` command: `npm i --global nmrium-cli`.

Once done from a command line move to the folder containing the exercises and execute the command `nmrium toc`.


## Publish on gh-pages



## Testing your exercises

https://www.nmrium.org/teaching#?toc=https://cheminfo.github.io/nmr-dataset-sample/toc.json

Each folder contains its own toc.json file so that you can directly give to you student the link to a subfolder

https://www.nmrium.org/teaching#?toc=https://cheminfo.github.io/nmr-dataset-sample/10_1D/10_60-12-8/toc.json
