# Running Denoising Notebooks: Instructions

- All notebooks depend on the `echopype` project
- The notebooks provided in the `noise tasks -echopype` folder should be copied into `/echopype/notebooks` before running them. When running the notebooks, all corresponding noise mask identification files (`mask_attenuated_signal.py`, `mask_range.py`, `mask_transient_noise.py`, `mask_seabed.py`, `mask_impulse_noise.py`) must be present in the mask module from `echopype/echopype/mask`. Additionally, `mask_transformation.py` must be present in the utils module from `echopype/echopype/utils`.
- Noise tasks notebooks:

    - `impulse_noise_mask.ipynb`
    - `range_mask.ipynb`
    - `seabed_mask.ipynb`
    - `signal_attenuation_mask.ipynb`
    - `transient_noise_mask.ipynb`