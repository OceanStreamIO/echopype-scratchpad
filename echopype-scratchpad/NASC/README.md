# Running NASC Notebooks: Instructions

- All notebooks depend on the `echopype` project
- The notebooks provided in the `NASC` folder should be copied into `/echopype/notebooks` before running them. When running the notebooks, the `mask_impulse_noise.py` file must be present in the mask module from `echopype/echopype/mask`. Additionally, `mask_transformation.py` must be present in the utils module from `echopype/echopype/utils`.
- NASC tasks notebooks:

    - `nasc_echopy_process_understanding.ipynb`  (Used for analyzing the Echopy code for NASC computation)
    - `nasc_echopype_process_understanding.ipynb`  (Used for analyzing Echopype code for NASC computation - where a bug was found)
    - `echopy-nasc-to-echopype-adaptation.ipynb` (Used for adapting the Echopy method for NASC computation to be suitable for Echopype, in case we need it in the future)