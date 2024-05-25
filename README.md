![Version](https://img.shields.io/static/v1?label=polyglotmolviz&message=0.0&color=brightcolor)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)


# Amalgamated molecular visualization on Colab

Code snippets to facilitate running several molecular graphics software packages in Colab notebooks.

Version 0.0.0


Chemists, biochemists, and pharmacologists frequently need to visualize the structures of both small and large molecules with molecular graphics software.
Historically, this software has been expensive and proprietary. 
However, open-source alternatives are now widely available. 
In addition, several Python packages support molecular visualization in Jupyter notebooks (e.g., /rdkit/, /nglview/, /py3dmol/, and /PyMOL/). 
The first package supports 2-D views of small molecules. 
The following two packages provide interactive 3-D views of small molecules and proteins. 
The fourth package provides static images of 3-D molecular scenes.
These images are of publication quality.
The first and last packages also support numerous kinds of structural analysis.

These packages can also operate in Colab. 
Google Colab provides a universally accessible computing platform. 
Universal access to the platform eliminates the problem of installing software on heterogeneous personal computers. 
This feature of Colab can save time and frustration for both instructors and students in laboratories, classrooms, and workshops. 
The user interacts with the cloud computing resources through an electronic computational notebook that runs in the web browser.
This electronic notebook is known as the Colab Notebook, a variant of the Jupyter Notebook. 
The latter has become the /de facto/ computing platform in scientific computing and data science.

The Colab notebook provides access to generic scientific computing packages preinstalled on Colab. 
This software includes widely used numerical computing packages like NumPy and pandas. 
If the required software is available on Colab, the user can import the packages or modules and execute code blocks in the notebook. 
Unfortunately, molecular graphics packages are not part of this software collection.

One solution to this issue is to install this software via Anaconda. 
However, Anaconda must be retrieved and installed in the correct location in Colab. 
These software installation steps are complex and take time if executed individually. 
This complexity can discourage new users.

To address the problem of adding molecular graphics software to Colab, we created code fragments that reduce these tasks to a single user click of an icon. 
We added these code fragments to snippet libraries for each molecular graphics package. 
The new libraries are called /colabrdkitsnips/, /colabpy3dmolsnips/, and /colabnglviewsnips/. 
In the case of PyMOL, we reformatted the published [[https://github.com/MooersLab/pymolsnips][pymolpysnips library]] for Colab and named it [[https://github.com/MooersLab/colabpymolpysnips][colabpymolpysnips]].
A [[https://github.com/MooersLab/colabOpenSourcePyMOLpySnips][variant]] of this library is available for use with OpenSource PyMOL, which does not require the loading of a PyMOL license file onto Google Drive.
(A description of the 250+ code snippets in the PyMOLsnips library is found [[https://mooerslab.github.io/pymolsnips/][here]].)

The installed software is lost when the user logs out of Colab. 
This loss is inconvenient because the installation step takes 6 - 8 minutes. 
Another code block archives the installed software as a tar file.
The code stores the tar file on the user's Google Drive. 
When the user logs into Colab again, a third code fragment retrieves the tar file and unpacks it in the correct location. 
This third step takes less than a minute and reduces the inconvenience of reinstalling software at the beginning of each Colab work session.

This work will be presented at SciPy 2022 in mid-July as abstract 222 and described in detail in a conference paper.

Mooers, B.H.M and Acquah, F.A. (2022)  Amalgamated molecular visualization on Colab.

This work was supported in part by the following grants:

- NIH: R01CA242845, R01AI088011, P20GM103640, P30CA225520, 3P30AG050911-07S1 
- Oklahoma Center for the Advancement of Science and Technology: HR20-002.

## Update history

|Version      | Changes                                                                                                                                     | Date                 |
|:-----------:|:------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------:|
| Version 0.0 |   Added badges, funding, and update table.                                                                                                 | 2024 May 24         |

## Sources of funding

- NIH: R01 CA242845
- NIH: R01 AI088011
- NIH: P30 CA225520 (PI: R. Mannel)
- NIH: P20 GM103640 and P30 GM145423 (PI: A. West)



