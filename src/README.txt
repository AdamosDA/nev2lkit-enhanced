==================================================================
This is a patched version of nev2lkit.

We chose to alter some parts of the program source code, in order 
to provide extended functionality to the feature extraction 
procedure. The following features were added, improving nev2lkit's 
spike-sorting capabilities.

1. Variable Length Data Window 
2. Variability of Principal Components
3. Calculation and Display of Variance
4. Spike Count in Each Cluster

This version of the patch is a production version. There is also 
a development version of this patch, which includes debugging 
functionality in order to monitor the PCA process at runtime. 

For further details regarding these features and the development 
version of this patch, you may visit:

http://neurobot.bio.auth.gr/nev2lkit

In order to install the patch:
- copy it to the root folder of nev2lkit 1.4 version
- execute "patch -p 0 < nev2lkit.patch"
- build as normal

Also, in order to properly compile the project, make sure that the
qwt library plugin (libqwtplugin.so) exists inside QT's plugin
directory (ex. /usr/lib/qt3/plugins/designer). If not, get QWT's
sources, compile the plugin according to installation instructions 
and install by hand.

The development of this work was made by Dr. Dimitrios A Adamos
(d.adamos@ieee.org) in the Laboratory of Animal Physiology, School
of Biology, Faculty of Science, Aristotle University. This work 
was implemented in the context of PYTHAGORAS II (EPEAEK) project,
a research program funded by the Greek Ministry of National 
Education and Religious Affairs.
==================================================================