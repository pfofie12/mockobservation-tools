# mockobservation_tools

These are tools I have created to aid in my research of Galaxy Simulations. Several of the tools are made to create mock images from the FIRE simulations and measure them using observation techniques, like Sersic Profiles Fiting. 

Several of the tools in galaxy_tools make use or are adapted from FIRE studio, a code created by Alex Gurvich https://ascl.net/2202.006
If using mockobservation_tools, please use my version of FIRE_studio, as I can ensure it is compatable with my mockobservation_tools:
https://github.com/courtk32/FIRE_studio

### To install FIRE_studio and mockobservation_tools:
To install these packages, you will git clone (or fork) the repositories to your local, then pip install them.
In you your local directory (does not matter where) git clone the two repositories

\texttt{git clone https://github.com/courtk32/FIRE_studio.git}
\texttt{git clone https://github.com/courtk32/mockobservation-tools.git}

\texttt{cd} into each of your cloned directory run:

\texttt{pip instal .}

For any updates in the code, update your repo and then your must run \texttt{pip instal .} to update your installed version


### How to use mockobservation_tools
Please review the tutorials notebooks.
Note that I have my own functions and examples for loading the data, however as long as the data is in dictionaries with the same labels you can use your method of loading your simulation.



### How to cite:
Citation for FIRE_studio (Gurvich 2022): https://ui.adsabs.harvard.edu/abs/2022ascl.soft02006G/abstract
Citation for Mockobservation_tools (Klein et al. 2024): https://doi.org/10.1093/mnras/stae1505 
Other citations:
(Hopkins et al. 2005)
(Hopkins et al. 2005)

### Example text:
We use an adapted version of \texttt{FIRE\textunderscore studio} (Hopkins et al. 2005; Gurvich 2022) to create mock images in SDSS $u$-, $g$- and $r$-bands, as described in Section 2.2 of (Klein et al. 2024). The luminosity of each star particle is derived using a mass-to-light ratio based on the particle's mass, age, and metallicity \citep{Chabrier2003GalacticFunction}. We take extinction into account via Thomson scattering, the photoelectric effect, and dust absorption \citep{Hopkins2005ALifetimes}. Each particle is smoothed using a cubic spline kernel with a smoothing length of 1.4 times the particle's gravitational softening length. 

You can also specify the Field of View, pixels size of image, or pixel scale (2 * FOV / npixels).
