# First 3C279 EHT Results: Calibrated Data

**Authors:** Kim et al.

**Date:** August 12th, 2020

**Primary Reference:** [Kim et al. 2020, A&A, 640, A69](https://doi.org/10.1051/0004-6361/202037493)

**Data Product Code:** [2020-D01-01](https://eventhorizontelescope.org/for-astronomers/data)

**Brief Description:**

We release a data set to accompany the *First 3C279 Event Horizon Telescope
Results* paper (Kim et al. 2020). The data set is derived from the Science
Release 1 (SR1) of the Event Horizon Telescope (EHT)'s April 2017 observation
campaign (EHTC et al. 2019).

This data set contains 3C279 data for both low and high bands for all observed
days (April 5th, 6th, 10th, 11th, 2017). Data from the 2017 observations were
processed through three independent reduction pipelines (Blackburn et al. 2019,
Janssen et al. 2019, EHTC et al. 2019). This release includes the fringe fitted,
a-priori calibrated, and network calibrated data from the EHT-HOPS pipeline,
which is the primary data set for the First 3C279 EHT results. Independent flux
calibration is performed based on estimated station sensitivities during the
campaign (Issaoun et al. 2017, Janssen et al. 2019). A description of the data
properties, their validation, and estimated systematic errors is given in EHTC
et al. (2019) with additional details in Wielgus et al. (2019).

The data are time averaged to 10 seconds and frequency averaged over all 32
intermediate frequencies (IFs). All polarization information is explicitly
removed. To make the resulting `uvfits` files compatible with popular
very-long-baseline interferometry (VLBI) software packages, the circularly
polarized cross-hand visibilities `RL` and `LR` are set to zero along with
their errors, while parallel-hands `RR` and `LL` are both set to an estimated
Stokes *I* value. Measurement errors for `RR` and `LL` are each set to sqrt(2)
times the statistical errors for Stokes *I*.

All `uvfits` files are located in the "`uvfits/`" subdirectory. Easy-to-read
`csv` and `txt` files are derived from the `uvfits` files and provided in
"`csv/`" and "`txt/`", respectively. Scripts that generate these files from the
original SR1 data are also included. Finally, the `run.sh` script in the top
directory will convert `uvfits` files into `csv` and `txt` files.

The three `tgz` files are gzipped tarballs that contains `uvfits`, `txt`, and
`csv` files, respectively. They are included in this repository for convenience.

**File Name Convention:**

The data files are named in the following convention:

    [Data-Release-Tag]_[Source]_[year]_[day-of-year]_[band]_[pipeline]_[stage]_StokesI.[format]

**Station Code Table:**

| UVFITS Code | Station Name                  | Location   |
| ----------- | ----------------------------- | ---------- |
| AA          | ALMA                          | Chile      |
| AP          | APEX                          | Chile      |
| AZ          | Submillimeter Telescope       | Arizona    |
| JC          | James Clerk Maxwell Telescope | Hawai'i    |
| LM          | Large Millimeter Telescope    | Mexico     |
| PV          | IRAM                          | Spain      |
| SM          | Submillimeter Array           | Hawai'i    |
| SP          | South Pole Telescope          | South Pole |

**References:**

- [EHT Collaboration Data Portal Website](https://eventhorizontelescope.org/for-astronomers/data)
- [EHTC et al. 2019, ApJL, 875, L3](https://doi.org/10.3847/2041-8213/ab0c57)
- [Blackburn, L., Chan, C.-k., Crew, G., et al. 2019, ApJ, 882, 23](https://ui.adsabs.harvard.edu/abs/2019ApJ...882...23B/abstract)
- [Janssen, M., Goddi, C., van Bemmel, I., et al. 2019, A&A, 626, A75](https://ui.adsabs.harvard.edu/abs/2019A%26A...626A..75J/abstract)
- [Issaoun, S., Folkers, T., Blackburn, L., et al. 2017, EHT Memo 2017-CE-02](https://eventhorizontelescope.org/for-astronomers/memos)
- [Janssen, M., Blackburn, L., Issaoun, S., et al. 2019, EHT Memo 2019-CE-01](https://eventhorizontelescope.org/for-astronomers/memos)
- [Wielgus, M., Blackburn, L., Issaoun, S., et al. 2019, EHT Memo 2019-CE-02](https://eventhorizontelescope.org/for-astronomers/memos)
