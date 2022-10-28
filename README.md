# PHYS_391B
## All code used for my PHYS391 project, including manim animations.

List of installed (and required for my code) packages in the project conda env:
- Tensorflow
- Keras (automatically installed with Tensorflow)
- [pandas](https://pandas.pydata.org/docs/getting_started/install.html)
- [matplotlib](https://matplotlib.org/stable/users/installing/index.html)
- [skimage](https://scikit-image.org/docs/stable/install.html#install-via-conda)
- [patchify](https://pypi.org/project/patchify/) (This was already installed with numpy for me.)
- [geopandas](https://geopandas.org/en/stable/getting_started/install.html)
- [xarray](https://docs.xarray.dev/en/stable/getting-started-guide/installing.html#instructions)
- [rioxarray](https://corteva.github.io/rioxarray/stable/installation.html)
- [shapely](https://pypi.org/project/Shapely/) (This was installed, I think with geopandas.)
- [opencv2](https://docs.opencv.org/4.x/d2/de6/tutorial_py_setup_in_ubuntu.html) (Their tutorial didn't work for me,
  use `conda install -c conda-forge opencv` instead.)

For installing the cuda dependencies for GPU based deep learning acceleration:
Following Nvidia's [developer guide](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html):
- First install [CUDA toolkit](https://developer.nvidia.com/cuda-downloads)
- Since I already had the current version of my nvidia dpu driver installed, I had to run the above .run file using:
    `sudo sh ./cuda_11.7.1_515.65.01_linux.run --toolkit --silent --override` which seems to have worked fine.
- Now, after downloading cudnn, follow [these](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html#installlinux-deb) steps.
- Finally, install [tensorrt](https://docs.nvidia.com/deeplearning/tensorrt/archives/tensorrt-723/install-guide/index.html)
