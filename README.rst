Datasets used by the `kikuchipy <https://kikuchipy.org>`_ Python library for
processing and analysis of electron backscatter diffraction (EBSD) patterns.

See individual datasets for their license.

If you find a dataset useful, please cite the individual dataset's DOI, or the
kikuchipy library DOI, https://doi.org/10.5281/zenodo.3597646, if an individual
DOI is not available.

nickel_ebsd_large
-----------------
.. image:: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
  :target: https://creativecommons.org/licenses/by/4.0/
  :alt: CC BY 4.0
.. image:: https://zenodo.org/badge/doi/10.5281/zenodo.3265037.svg
  :target: https://doi.org/10.5281/zenodo.3265037
  :alt: DOI

- Origin: https://doi.org/10.5281/zenodo.3265037
- Description: A set of experimental EBSD patterns from a recrystallized 
  polycrystalline Nickel sample of (55 x 75) patterns of (60 x 60) pixels.

silicon_ebsd_moving_screen
--------------------------
.. image:: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
  :target: https://creativecommons.org/licenses/by/4.0/
  :alt: CC BY 4.0

- Origin: Acquired by Håkon Wiik Ånes and Jarle Hjelen at NTNU in 2021.
- Description: Three experimental EBSD patterns of (480 x 480) pixels from a
  single crystal Silicon sample acquired with a stationary beam but with
  camera distances varying by 5 mm.

pzt_pseudosym_ebsd
-------------------
.. image:: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
  :target: https://creativecommons.org/licenses/by/4.0/
  :alt: CC BY 4.0

- Origin: Acquired by Claire Griesbach at ETH Zurich in 2025. A subset of the 
  full dataset, which is available here: https://doi.org/10.3929/ethz-c-000799672
- Description: A (19 x 19) subset of experimental EBSD patterns of (169 x 169)
  pixels (2x2 binned, uint8) from a polycrystalline lead zirconium titanate (PZT) sample, 
  acquired on an TFS Quanta 200F SEM equipped with an EDAX Hikari camera mounted at an
  azimuthal angle of -2 degrees. The dataset also includes a dynamical EBSD master pattern 
  of PbZr0.52Ti0.48O3 at 15 kV accelerating voltage, simulated with Oxford Instrument's 
  AZtecCrystal MapSweeper software.``master_pattern.hspy`` is resaved in HyperSpy's own 
  HDF5 format from the original vendor export, since kikuchipy's EMsoft reader does not 
  recognize the original file's structure; load it with
  :func:`kikuchipy.data.pzt_pseudosym_ebsd_master_pattern`, which reapplies the
  hemisphere/projection/phase metadata that this format does not itself
  persist.
