About url-into-images
=====================

Home: https://github.com/sujitmandal/url-into-images

Package license: MIT

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/url-into-images-feedstock/blob/main/LICENSE.txt)

Summary: provide image download link through csv file and it will download all the images. also you can chose different extension.

Development: https://github.com/sujitmandal/url-into-images

Documentation: https://sujitmandal.github.io/url-into-images/

Current build status
====================


<table><tr><td>All platforms:</td>
    <td>
      <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=15778&branchName=main">
        <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/url-into-images-feedstock?branchName=main">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-url--into--images-green.svg)](https://anaconda.org/conda-forge/url-into-images) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/url-into-images.svg)](https://anaconda.org/conda-forge/url-into-images) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/url-into-images.svg)](https://anaconda.org/conda-forge/url-into-images) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/url-into-images.svg)](https://anaconda.org/conda-forge/url-into-images) |

[![Build Status](https://travis-ci.org/sujitmandal/url-into-images.svg?branch=master)](https://travis-ci.org/sujitmandal/url-into-images) [![GitHub license](https://img.shields.io/github/license/sujitmandal/url-into-images)](https://github.com/sujitmandal/url-into-images/blob/master/LICENSE) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/url-into-images) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/url-into-images) ![PyPI](https://img.shields.io/pypi/v/url-into-images) ![Conda Version](https://img.shields.io/conda/vn/conda-forge/url-into-images.svg) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/url-into-images/badges/version.svg)](https://anaconda.org/conda-forge/url-into-images) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/url-into-images/badges/installer/conda.svg)](https://conda.anaconda.org/conda-forge) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/url-into-images/badges/platforms.svg)](https://anaconda.org/conda-forge/url-into-images) [![Conda Recipe](https://img.shields.io/badge/recipe-url--into--images-green.svg)](https://anaconda.org/conda-forge/url-into-images) ![](https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/url-into-images-feedstock?branchName=main)

[![Downloads](https://pepy.tech/badge/url-into-images)](https://pepy.tech/project/url-into-images)


Installing url-into-images
==========================

Installing `url-into-images` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `url-into-images` can be installed with `conda`:

```
conda install url-into-images
```

or with `mamba`:

```
mamba install url-into-images
```

It is possible to list all of the versions of `url-into-images` available on your platform with `conda`:

```
conda search url-into-images --channel conda-forge
```

or with `mamba`:

```
mamba search url-into-images --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search url-into-images --channel conda-forge

# List packages depending on `url-into-images`:
mamba repoquery whoneeds url-into-images --channel conda-forge

# List dependencies of `url-into-images`:
mamba repoquery depends url-into-images --channel conda-forge
```


## Url Into Images :
provide image download link through csv file and it will download all the images. also you can chose different extension.
```
 • jpg

 • jpeg

 • png

 • bmp

 • gif
```
## How to import the module:
```python
URL_PATH = ('') # csv file where image URL contain

IMAGE_PATH = ('') # Download image path
```
## Download JPG
```python
from url_into_images.url_into_images import url_jpg

url_jpg(URL_PATH, IMAGE_PATH)
```
## Download JPEG
```python
from url_into_images.url_into_images import url_jpeg

url_jpeg(URL_PATH, IMAGE_PATH)
```
## Download PNG
```python
from url_into_images.url_into_images import url_png

url_png(URL_PATH, IMAGE_PATH)
```
## Download BMP
```python
from url_into_images.url_into_images import url_bmp

url_bmp(URL_PATH, IMAGE_PATH)
```
## Download GIF
```python
from url_into_images.url_into_images import url_gif

url_gif(URL_PATH, IMAGE_PATH)
```

## Required package’s:
```
• pip install pandas
```

About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [Anaconda-Cloud](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating url-into-images-feedstock
==================================

If you would like to improve the url-into-images recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/url-into-images-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@sujitmandal](https://github.com/sujitmandal/)

