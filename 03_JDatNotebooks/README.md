This directory holds materials for the JWST Data Analysis Science Workflow Hack Hour

Be sure to ``conda activate aas239-jwebbinar`` before running any materials.

Here is a summary of the notebooks you can try.

| Notebook Name   | Description | Instrument | Packages |
| ----------- | ----------- | ----------- | ----------- |
| IFU_cube_continuum_fit     |   Subtract continuum and emission-line modeling of AGN in a 3D cube environment.  |  Gemini data/cross-instrument | specutils, jdaviz/cubeviz  |
| MRS_Mstar_analysis   | Extract spatial-spectral features from MIRI MRS IFU cube, subtract blackbody continuum, and measure lines.  | Simulated MIRI data/cross-instrument |  specutils, jdaviz/specviz  |
| background_estimation_imaging   | Estimate the sky background in complex scenes and evaluate the quality of the sky estimation.  | Fake NDARRAY data/cross-instrument | jdaviz/imviz | 
| spec_analysis   |  Three examples on how a user can measure the redshift of a source.   | Simulated NIRISS spectrum/cross-instrument | specutils, jdaviz/specviz |