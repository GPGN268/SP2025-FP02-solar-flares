# ☀️ SP2025-FP02-solar-flares ☀️

## Erica Maebius (emaebius) and Anna Williams (ag-williams)

### Short 1-2 sentence summary
Solar flares, caused by the tangling of the sun's magnetic field, eject large amounts of electromagnetic energy into space. Although Earth's atmosphere protects us from the majority of emitted charged particles and X-rays, solar flares can disrupt the ionosphere, impacting radio wave propagation around the world. This can be problematic for satellite and air traffic communications. We will analyze a report, "Super-Intense Geomagnetic Storm on 10–11 May 2024: Possible Mechanisms and Impacts" and attempt to recreate their charts based on the open source data provided.

### Some introductory background information
- The equatorial and polar areas of the Sun rotate at different rates, which causes the Sun's magnetic fields to tangle. [1]
- At these tangled spots, the localized magnetic field can become so strong that they twist away from the Sun's surface, ejecting large amounts of radiation. [1]
- These ejections create solar storms. [1]
- Solar storms come in a couple of different flavors: [2]
    - Solar flares, which are an intense burst of electromagnetic radiation. These range from A (weakest), B, C, M, X(strongest). These classes are on a logarithmic scale. Within each class, they are further subdivided into 1-9.
        - Energy from flares travel at the speed of light!
    - Radiation storms are explosions of electrically charged particals (protons and electrons).
    - Coronal mass ejections (CMEs) occur when plasma (electrically charged gas) erupts from the sun. These are much slower than solar flares and radiation storms but have a much larger impact on Earth. They can induce electrical currents and damage electrical equipment and heat up the atmosphere, increasing drag on orbiting satellites.


### Problem statement, question(s) and/or objective(s)
- Can we predict when a solar storm effects on wave disruptions?
- Can we model how a solar storm will impact radio or satellite communications?
- Can we model how the ionosphere is affected by solar storms?

### Datasets you will use (with links, if available)
- [Geomagnetic Storm Report](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2024SW004126#swe21812-bib-0020)
- [DSCOVR Solar Wind and IMF Data](https://www.ngdc.noaa.gov/dscovr/portal/index.html#/download/)
- [Sym-H Index Data](http://wdc.kugi.kyoto-u.ac.jp/aeasy/index.html)
- [GOES-18 Magnetic Field Data](https://cdaweb.gsfc.nasa.gov/pub/data/goes/goes18/)
- [Global TEC Maps from GNSS Receiver Network](http://millstonehill.haystack.mit.edu/listExperiments?isGlobal=on&categories=17&instruments=8000&showDefault=on&start_date_0=1950-01-01&start_date_1=00%3A00%3A00&end_date_0=2024-12-31&end_date_1=23%3A59%3A59)
- [Solar Wind Dynamic Pressure, IMF Bz, and Sym-H Data](https://omniweb.gsfc.nasa.gov/form/omni_min_def.html)
- [Magnetometer, VLF Receiver, and Ionosonde Data](https://doi.org/10.5281/zenodo.12623351)
- [BATSRUS Model Simulation Data](https://ccmc.gsfc.nasa.gov/results/viewrun.php?runnumber=Nilam_Bhosale_071124_1)

### Tools/packages you’ll use (with links)
- [Matplotlib](https://matplotlib.org/stable/) (pyplot for sure)
- [Numpy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)
- [Seaborn](https://seaborn.pydata.org/) 

### Planned methodology/approach
We will use the publicly available datasets provided in the May 10-11 storm report in order to analyze, evaluate, and recreate the graphs.

### Present or anticipated challenges
- The datasets are very large and will require downsizing which may alter our ability to recreate the graphs.
- There are many different forms of data that are also recorded in different ways that will requiring significant preprocessing and cleaning.
- The substantial length and depth of the report may go beyond our ability and timescale of this project and may call for downsizing.

### Expected outcomes
We hypothesize that we will see a positive correlation between mass ejection APIs and recorded radio wave frequency disruptions. Additionally, we predict that a smaller solar flare will be less damaging to the ionosphere and have less widespread consequences.

### Any other relevant information, images/tables, references, etc.
[NOAA's Space Weather Prediction Website](https://www.swpc.noaa.gov/phenomena/coronal-mass-ejections)

### References
[1] https://scied.ucar.edu/video/sun-magnetic-field-rotate-tangle-movie
[2] https://science.nasa.gov/sun/solar-storms-and-flares/
[3] https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2024SW004126#swe21812-bib-0020
