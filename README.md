# ☀️ SP2025-FP02-solar-flares ☀️

## Erica Maebius (emaebius) and Anna Williams (ag-williams)

### Summary
Solar flares, caused by the tangling of the sun's magnetic field, eject large amounts of electromagnetic energy into space. Although Earth's atmosphere protects us from the majority of emitted charged particles and X-rays, solar flares can disrupt the ionosphere, impacting radio wave propagation around the world. This can be problematic for satellite and air traffic communications. We will analyze a report, "Super-Intense Geomagnetic Storm on 10–11 May 2024: Possible Mechanisms and Impacts" and attempt to recreate their charts based on the open source data provided.

### How to Use This Repository
An in depth project report is written in the report.ipynb file found in the notebooks folder. This includes information on what data we used, beautiful visualizations, and descriptions of what they mean. For a more in depth look at how the visualizations were created, the notebook files responsible for each plot are also available in the notebooks folder. To just view the developed figures, see the figures folder. The dev folder contains uncleaned process notebooks and a bloopers notebook.

### Background
The sun, composed of plasma, rotates at different rates in the polar (slower) and equatorial (faster) regions. This differentiation in the speed of rotation causes the Sun's magnetic fields to tangle. At these tangled spots, the localized magnetic field can become so strong that they twist and explode away from the Sun's surface ejecting large amounts of particles and radiation [1]. Different types of solar weather include radiation storms, solar flares, and coronal mass ejections. Radiation storms are explosions of electrically charged particles (protons and electrons). Solar flares are an intense burst of electromagnetic radiation. These range from A (weakest), B, C, M, X (strongest). These classes are on a logarithmic scale. Within each class, they are further subdivided into a magnitude of 1-9. Solar flares are an explosive ejection of electromagnetic energy. Coronal mass ejections (CMEs) occur when plasma (electrically charged gas) erupts from the sun. These are much slower than solar flares and radiation storms but have a much larger impact on Earth. They can induce electrical currents and damage electrical equipment and heat up the atmosphere, increasing drag on orbiting satellites [2]. The May 2024 storm contained a combination of all three.


### Research Questions
- What impacts did the May 2024 solar storm have on radio communication and the conditions of the ionosphere?
- How did the solar storm evolve over May 10th and May 11th?

### Datasets
- [Geomagnetic Storm Report](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2024SW004126#swe21812-bib-0020)
- [DSCOVR Magnetic Field and Proton Data](https://www.ngdc.noaa.gov/dscovr/portal/index.html#/download/)
- [GOES-18 Magnetic Field Data](https://cdaweb.gsfc.nasa.gov/pub/data/goes/goes18/)
- [Global TEC Maps from GNSS Receiver Network](http://millstonehill.haystack.mit.edu/listExperiments?isGlobal=on&categories=17&instruments=8000&showDefault=on&start_date_0=1950-01-01&start_date_1=00%3A00%3A00&end_date_0=2024-12-31&end_date_1=23%3A59%3A59)
- [Magnetometer, VLF Receiver, and Ionosonde Data](https://doi.org/10.5281/zenodo.12623351)

### Tools/packages you’ll use (with links)
- [Matplotlib](https://matplotlib.org/stable/)
- [Numpy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)
- [Xarray](https://docs.xarray.dev/en/stable/)
- [Cartopy](https://scitools.org.uk/cartopy/docs/latest/)
- [SciPy](https://scipy.org/)
- [NetCDF4](https://unidata.github.io/netcdf4-python/)

### Methodology
We used the publicly available datasets provided in the May 10-11 storm report to analyze, evaluate, and recreate the graphs. After locating the needed datafiles, many of which were in alternative forms to ".csv", we loaded the needed data into notebooks. After preprocessing the data and proceeding with Exploratory Data Analysis, we began trying to reconstruct the graphs (based on their respective data) to the best of our abilities. Based on our constructions combined with external research we then interpreted the plots and gathered the key insights they provided.

### Challanges
In our attempts to recreate many of the graphs present in the "Super-Intense Geomagnetic Storm on 10–11 May 2024: Possible Mechanisms and Impacts" report, we encountered many complications. Some of the cited "Open Research" sources were wholly inaccessible or very difficult to locate. Additionally, the few datasets we were able to acquire were organized in different ways and data formats. For example, in just Figure 1 and Figure 2, there were three different file formats, ".nc", ".txt", and ".csv". Even after opening the data and transforming them into datasets or dataframe's issues remained, whether it be with excessive missing values, incorrectly parsed files, or variations in column and feature names. 

When attempting to match our graphs to that of the report, many of the data points did not correspond. This could have been a result of smoothing of the plots on the official reports side, or differences in the preprocessing steps.

### Statement of Contribution
Both group members contributed to the interpretations and conceptual analysis of the graphs and their application to the overall investigation. Erica primarily worked on the GOES and DSCOVR magnetic field graph and the VLF and equatorial electrojet graph. Anna constructed the DSCOVR magnetic field and proton plots and the TEC map.

### References
[1] https://scied.ucar.edu/video/sun-magnetic-field-rotate-tangle-movie

[2] https://science.nasa.gov/sun/solar-storms-and-flares/

[3] https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2024SW004126#swe21812-bib-0020
