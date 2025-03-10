# SP2025-FP02-solar-flares
Final project repo for the solar flare analysis group

# ☀️ Solar Flares ☀️

## Erica Maebius (emaebius) 😊 and Anna Williams (ag-williams) 😊

### Short 1-2 sentence summary
Solar flares, caused by the tangling of the sun's magnetic field, eject large amounts of electromagnetic energy into space. Although Earth's atmosphere protects us from the majority of emitted charged particles and x-rays, solar flares candisrupt the ionosphere impacting radio wave propagation around the world. This can be problematic for satellite and air traffic communications. We will use NASA’s solar flare and coronal mass ejection APIs as our data on the solar flares. We can then cross reference this material to known radio wave frequency disruptions to determine the impact of the solar flares.

### Some introductory background information
- The equatorial and polar areas of the Sun rotate at different rates which cause the Sun's magnetic fields to tangle. [1]
- At these tangle spots, the localized magnetic field can become so strong that they twist away from the Sun's surface ejecting large amount of radiation. [1]
- These ejections create solar storms. [1]
- Solar storms come in a couple different flavors: [2]
    - Solar flares which are an intense burst of electromagnetic radiation. These range on a scale of (A (weakest),B,C,M,X(strongest)). These classes are on a logarithmic scale. Within each class, they are further subdivided into 1-9.
        - Energy from flares travel at the speed of light!
    - Radiation storms are explosions of electrically charged particals (protons and electrons).
    - Coronal mass ejections (CMEs) occur when plasma (electrically charged gas) erupts from the sun. These are much slower than solar flares and radiation storms but have a much larger impact on Earth. They can induce electrical currents and dammage electrical equipment and heat up the atmosphere increasing drag on orbiting satelites.


### Problem statement, question(s) and/or objective(s)
- Can we predict when a solar storm will occur and at what intensity?
- Can we model how a solar storm will impact radio or satelite communications?
- Can we model how the ionosphere is affected by solar storms?

### Datasets you will use (with links, if available)
- [DONKI](https://ccmc.gsfc.nasa.gov/tools/DONKI/)
- [SWPC Data](https://www.swpc.noaa.gov/content/data-access)

### Tools/packages you’ll use (with links)
- [Matplotlib](https://matplotlib.org/stable/) (pyplot for sure)
- [Numpy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)
- [Seaborn](https://seaborn.pydata.org/) :)

### Planned methodology/approach
We will use NASA’s solar flare and coronal mass ejection APIs as our data on the solar flares. We can then cross reference this material to known radio wave frequency disruptions to determine the impact of the solar flares.

### Expected outcomes
We hypothesize that we will see a positive correlation between mass ejection APIs and recorded radio wave frequency disruptions. Additionally, we predict that a smaller solar flare will be less damaging to the ionosphere and have less widespread consequences.

### Any other relevant information, images/tables, references, etc.
[NOAA's Space Weather Prediction Website](https://www.swpc.noaa.gov/phenomena/coronal-mass-ejections)

### References
[1] https://scied.ucar.edu/video/sun-magnetic-field-rotate-tangle-movie
[2] https://science.nasa.gov/sun/solar-storms-and-flares/
