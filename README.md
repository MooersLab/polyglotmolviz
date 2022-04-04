# polyglotmolviz
Code snippets to facilitate running several molecular graphics software packages in Colab notebooks.

Version 0.0.0


Chemists, biochemists, and pharmacologists frequently need to visualize the structures of both small and large molecules with molecular graphics software. Historically, this software has been expensive and proprietary. 
However, open-source alternatives are now widely available. 
In addition, several python packages support molecular visualization in Jupyter notebooks (e.g., rdkit, nglview, py 3 dmol, and PyMOL.). 
The first package supports 2-D views of small molecules. 
The following two packages provide interactive 3-D views of small molecules and proteins. 
The fourth package provides static images of 3-D molecular scenes that are of publication quality.
The first and last packages also support numerous kinds of structural analysis in addition to molecular visualization.

These packages can also operate in Colab. 
Google Colab provides a universally accessible computing platform. 
Universal access to the platform eliminates the problem of installing software on heterogeneous personal computers. 
This feature of Colab can save time and frustration for both instructors and students in laboratories, classrooms, and workshops. 
The user interacts with the cloud computing resources by interacting with an electronic computational notebook known as the Colab Notebook, which is related to the Jupyter Notebook. 
The latter has become the de facto computing platform in scientific computing.

The Colab notebook provides access to generic scientific computing packages preinstalled on Colab. 
This software includes widely used numerical computing packages like NumPy and pandas. 
If the required software is already available on Colab, the user can import the packages or modules and start executing code blocks in the notebook. 
Unfortunately, molecular graphics packages are not part of this software collection.

One solution to this issue is to install this software via Anaconda. 
However, Anaconda must be retrieved and installed in the correct location in Colab. 
These software installation steps are complex and take time if executed individually. 
This complexity can discourage new users.

To address this and other problems with adding software to Colab, we created code fragments that reduce these tasks to a single click of an icon by the user. 
We added these code fragments to snippet libraries for each molecular graphics package. 
The new libraries are called colabrdkit, colabpy3dmolsnips, and colabnglviewsnips. 
In the case of PyMOL, we reformatted the published pymolpysnips library for Colab and named colabpymolpysnips.

The installed software is lost when the user logs out of Colab. 
This loss is inconvenient because the installation step takes 6 - 8 minutes. 
A second code fragment archives the installed software as a tar file and stores the tar file on the user's Google Drive. 
A third fragment retrieves the tar file and unpacks it in the correct location after the user logs into Colab again. 
This third step takes less than a minute and reduces the inconvenience of reinstalling software at the beginning of each Colab work session.


This work was support in part by the following grants:

NIH: R01CA242845, R01AI088011, P20GM103640, P30CA225520, 3P30AG050911-07S1 and the Oklahoma Center for the Advancement of Science and Technology HR20-002.




