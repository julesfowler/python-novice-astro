---
layout: lesson
root: .
---

The best way to learn how to program is to do something useful,
so this introduction to Python is built around a common scientific task:
**data analysis**.

### Supernovae Lighcurves

A [supernova](https://en.wikipedia.org/wiki/Supernova) is a tremendous stellar explosion. A supernova is a transient event which occurs at the end of life of a massive star or when a white dwarf is triggered into a runaway nuclear reaction. The light curve of a supernova is constructed by plotting its magnitude as a function of time. At the peak of its brightness a supernova can outshine its host galaxy but its light quickly fades away. More detailed information about light curves can be found [here]
(http://astronomy.swin.edu.au/cosmos/T/Type+Ia+Supernova+Light+Curves).

We are studying supernova lighcurves measured in a four bandpasses - g, r, i and z.
The data in this tutorial comes from [Guy et al., (2010)](https://ui.adsabs.harvard.edu/?#abs/2010A%26A...523A...7G).
The observations of 231 high-redshift supernovae are split into separate files in the 
[comma-separated values]({{ page.root }}/reference/#comma-separated-values) (CSV) format:

- each row holds information for a single day of observations,
- columns represent different filters.

The first three rows of our first file look like this:
~~~
MJD,Flux_g,e_Flux_g,Flux_r,e_Flux_r,Flux_i,e_Flux_i,Flux_z,e_Flux_z
52880.5,13.035,5.4246,NaN,NaN,NaN,NaN,NaN,NaN
52881.5,NaN,NaN,7.0282,9.9105,16.157,18.629,22.086,71.951
52886.6,NaN,NaN,NaN,NaN,189.44,19.855,NaN,NaN
~~~
{: .source}

So, we want to:

1. Calculate the maximum brightness in each band.
2. Plot the light curves to discuss and share with colleagues.

To do all that, we'll have to learn a little bit about programming.

> ## Prerequisites
>
> You need to understand the concepts of **files** and **directories** and how to start a Python
> interpreter before tackling this lesson. This lesson sometimes references Jupyter
> Notebook although you can use any Python interpreter mentioned in the [Setup](setup/).
>
> The commands in this lesson pertain to **Python 3**.
{: .prereq}

### Getting Started
To get started, follow the directions on the "[Setup](setup/)" page to download data
and install a Python interpreter.
