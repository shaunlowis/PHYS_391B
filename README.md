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
`https://storage.googleapis.com/tensorflow/linux/gpu/tensorflow_gpu-2.10.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl`\

List of installed packages in the tf conda env:
- Tensorflow
- Keras
