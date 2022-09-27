# PHYS_391B

For now just using this to document my keras installation, since it is scary and I am scared.\
Using this command to install appropriate NVIDIA driver for my rtx3060:\
`sudo apt install nvidia-driver-470`


Apparently the next step is to then go:\
`sudo prime-select nvidia`


Okay so it seems to have worked,running:\
`nvidia-smi`

produces:


![Screenshot from 2022-09-27 15-06-20](https://user-images.githubusercontent.com/63687545/192414592-c6c52f35-4997-49cd-9355-6100b0bdca62.png)


now I just need to follow the rest of [this](https://www.tensorflow.org/install/pip) guide.
According to the guide, there may be some need to use the install link, which is:\
`https://storage.googleapis.com/tensorflow/linux/gpu/tensorflow_gpu-2.10.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl`

I used [the following link](https://data.linz.govt.nz/x/vGMekh) to download my data.

List of installed (and required for my code) packages in the tf conda env:
- Tensorflow
- Keras (automatically installed with Tensorflow)
- [pandas](https://pandas.pydata.org/docs/getting_started/install.html)
- [matplotlib](https://matplotlib.org/stable/users/installing/index.html)
- [skimage](https://scikit-image.org/docs/stable/install.html#install-via-conda)
- [patchify](https://pypi.org/project/patchify/) (This was already installed with numpy for me.)
- [geopandas](https://geopandas.org/en/stable/getting_started/install.html)
- [xarray](https://docs.xarray.dev/en/stable/getting-started-guide/installing.html#instructions)
- [rioxarray](https://corteva.github.io/rioxarray/stable/installation.html)
- [shapely](https://pypi.org/project/Shapely/)(This was installed, I think with geopandas.)

Next step is to apply the [Sobel operator](https://www.youtube.com/watch?v=uihBwtPIBxM) on the older data after retraining my model.\
The main reason I think it is necessary to retrain the model is because the true positive reading was at the low end of 70% and it will
form the basis of all of our investigative work into the growth projection "turing model" which we are developing, so it is probably best to not build on sand if at all avoidable.
