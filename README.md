# nev2lkit-enhanced
Nev2lkit enhanced can sort successfully larger amount of spikes and adapt to low SNRs.

[Nev2lkit](http://nev2lkit.sourceforge.net) is a preprocessor for the analysis of extracellular neuronal recordings developed by Daniel Micol.

Herein, this enhanced version incorporates new features to Nev2lkit’s source code, in order to provide enhanced functionality to the spike sorting process. In summary, the following features were added:

1. Variable Length Data Window 
The ability of applying Principal Component Analysis on a variable-length data window was implemented, following 0.1 ms accuracy. The data window defines the spike waveform length that is taken into account in the spike extraction process and afterwards inserted into PCA. With this feature, the software can adopt in variable-length spiking activity and avoid the insertion of artifacts.

2. **Variability of Principal Components**
The ability to select the number of principal components used to perform spike waveform representation by PCA, was also added. The number of engaging principal components (between 2 & 7) can now be selected.

3. **Calculation and Display of Variance**
In spike waveform representation by the principal components, the percentage variance captured by that subspace is computed and displayed in the program’s graphical interface.

4. **Spike Count in Each Cluster**
Besides the total count of the detected spikes by the extraction process, the ability of displaying the number of spikes assigned to each cluster (as an additional output of the clustering process), was added.
