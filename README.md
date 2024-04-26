# Principles of Data Analytics project 2024

<img src="https://allisonhorst.github.io/palmerpenguins/reference/figures/lter_penguins.png" alt="A cartoon image of the Chinstrap, Gentoo, and Adélie species of penguin." width="600">

This repository contains my analysis of the famous [Palmer Penguins dataset](https://allisonhorst.github.io/palmerpenguins/) (Horst AM, Hill AP, Gorman KB 2020). The data is shared under a [CC-0 license](https://creativecommons.org/public-domain/cc0/) which allows it to be freely used, to foster research and analysis. I utilised the [dataset found here](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/penguins.csv) for the purposes of my analysis.

This analysis was carried out for the [Principles of Data Analytics](https://www.gmit.ie/principles-of-data-analytics) module as part of the [Higher Diploma in Science in Data Analytics at ATU](https://www.gmit.ie/higher-diploma-in-science-in-computing-in-data-analytics).

## Modules
I made use of the following modules as part of this project.
- [pandas](https://pandas.pydata.org/)
- [pyplot](https://matplotlib.org/3.5.3/api/_as_gen/matplotlib.pyplot.html)
- [seaborn](https://seaborn.pydata.org/tutorial/introduction.html)
- [numpy](https://numpy.org/)
- [warnings](https://docs.python.org/3/library/warnings.html)

## Dataset
The dataset contains measurements for 344 penguins spread over three islands on the Palmer Archipelego, [a group of islands off the northwestern coast of the Antarctic Peninsula](https://en.wikipedia.org/wiki/Palmer_Archipelago). The [full dataset](https://cloud.r-project.org/web/packages/palmerpenguins/index.html) contains various data points including Region, Egg Stage, Individual ID, and further comments. For the purposes of this analysis, I will be working with a simplified dataset which contains the following variables only:
- **species:** Adélie, Chinstrap, or Gentoo
- **island:** Biscoe, Dream, or Torgersen
- **bill_length_mm:** length (in mm) of the penguin's culmen (upper ridge of the penguin's bill)
- **bill_depth_mm:** depth (in mm) of the penguin's culmen
- **flipper_length_mm:** length (in mm) of the penguin's flipper
- **body_mass_g:** body mass (in g) of the penguin
- **sex:** whether the penguin was Female or Male

## Datatypes
The dataset contains two [primary datatypes](https://pbpython.com/pandas_dtypes.html) - **objects** and **float64s**.
- **species:** object
- **island:** object
- **bill_length_mm:** float64
- **bill_depth_mm:** float64
- **flipper_length_mm:** float64
- **body_mass_g:** float64
- **sex:** object

Species and Island are objects with three variables each. Sex is also an object, but given that it has two options and is a binary choice (excluding any considerations about intersex penguins), we could convert this into a bool variable if we wished (under the heading **Is Female**, the data could be *True* or *False*).

The remaining datatypes are all floats and describe measurements of various penguin body parts.

## References
- All artwork used is by [@allison_horst](https://twitter.com/allison_horst)
- [Horst AM, Hill AP, Gorman KB (2020). palmerpenguins: Palmer Archipelago (Antarctica) penguin data](https://allisonhorst.github.io/palmerpenguins/)