# TensorFlow Optimized Wheels

Custom builds for TensorFlow with platform optimizations, including SSE, AVX and FMA. If you are seeing messages like the following with the stock `pip install tensorflow`, you've come to the right place.

```
The TensorFlow library wasn't compiled to use AVX instructions, but these are available on your machine and could speed up CPU computations.
The TensorFlow library wasn't compiled to use SSE4.1 instructions, but these are available on your machine and could speed up CPU computations.
...
```

These wheels are built for use on [TinyMind](https://www.tinymind.com), the cloud machine learning platform. If you want to install them on your own Linux box (Ubuntu 16.04 LTS), you can do so with:

```sh
# RELEASE is the git tag like tf1.1-cpu. WHEEL is the full wheel name.
pip --no-cache-dir install https://github.com/mind/wheels/releases/download/{RELEASE}/{WHEEL}
```

If you want a shorter URL, use:

```sh
pip --no-cache-dir install http://wheels.tinymind.org/{RELEASE}/{WHEEL}
```

The list of all wheels can be found in the [releases page](https://github.com/mind/wheels/releases).

## Versions

The table below lists versions you will most likely use. However, be sure to check out the [releases page](https://github.com/mind/wheels/releases) as we are adding other builds (debug, XLA, MPI, etc) to the collection. Need something or a wheel doesn't work for you? File an issue.

Please note that your machine needs to have a relatively new Intel CPU (and Nvidia GPU if you use the GPU version) to be compatible with the wheels below. If the hardware is not up-to-date, the wheels will not work.

See the section below for information about CUDA support.

Version | Python | Arch | Link
--------|--------|------|-----
1.1 | 2.7 | CPU | https://github.com/mind/wheels/releases/download/tf1.1-cpu/tensorflow-1.1.0-cp27-cp27mu-linux_x86_64.whl
1.1 | 3.5 | CPU | https://github.com/mind/wheels/releases/download/tf1.1-cpu/tensorflow-1.1.0-cp35-cp35m-linux_x86_64.whl
1.1 | 3.6 | CPU | https://github.com/mind/wheels/releases/download/tf1.1-cpu/tensorflow-1.1.0-cp36-cp36m-linux_x86_64.whl
1.1 | 2.7 | GPU | https://github.com/mind/wheels/releases/download/tf1.1-gpu/tensorflow-1.1.0-cp27-cp27mu-linux_x86_64.whl
1.1 | 3.5 | GPU | https://github.com/mind/wheels/releases/download/tf1.1-gpu/tensorflow-1.1.0-cp35-cp35m-linux_x86_64.whl
1.1 | 3.6 | GPU | https://github.com/mind/wheels/releases/download/tf1.1-gpu/tensorflow-1.1.0-cp36-cp36m-linux_x86_64.whl
1.2 | 2.7 | CPU | https://github.com/mind/wheels/releases/download/tf1.2-cpu/tensorflow-1.2.0-cp27-cp27mu-linux_x86_64.whl
1.2 | 3.5 | CPU | https://github.com/mind/wheels/releases/download/tf1.2-cpu/tensorflow-1.2.0-cp35-cp35m-linux_x86_64.whl
1.2 | 3.6 | CPU | https://github.com/mind/wheels/releases/download/tf1.2-cpu/tensorflow-1.2.0-cp36-cp36m-linux_x86_64.whl
1.2 | 3.6 | GPU | https://github.com/mind/wheels/releases/download/tf1.2-gpu/tensorflow-1.2.0-cp36-cp36m-linux_x86_64.whl
1.2.1 | 2.7 | CPU | https://github.com/mind/wheels/releases/download/tf1.2.1-cpu/tensorflow-1.2.1-cp27-cp27mu-linux_x86_64.whl
1.2.1 | 3.5 | CPU | https://github.com/mind/wheels/releases/download/tf1.2.1-cpu/tensorflow-1.2.1-cp35-cp35m-linux_x86_64.whl
1.2.1 | 3.6 | CPU | https://github.com/mind/wheels/releases/download/tf1.2.1-cpu/tensorflow-1.2.1-cp36-cp36m-linux_x86_64.whl
1.2.1 | 2.7 | GPU | https://github.com/mind/wheels/releases/download/tf1.2.1-gpu/tensorflow-1.2.1-cp27-cp27mu-linux_x86_64.whl
1.2.1 | 3.5 | GPU | https://github.com/mind/wheels/releases/download/tf1.2.1-gpu/tensorflow-1.2.1-cp35-cp35m-linux_x86_64.whl
1.2.1 | 3.6 | GPU | https://github.com/mind/wheels/releases/download/tf1.2.1-gpu/tensorflow-1.2.1-cp36-cp36m-linux_x86_64.whl
1.3 | 2.7 | CPU | https://github.com/mind/wheels/releases/download/tf1.3-cpu/tensorflow-1.3.0-cp27-cp27mu-linux_x86_64.whl
1.3 | 3.5 | CPU | https://github.com/mind/wheels/releases/download/tf1.3-cpu/tensorflow-1.3.0-cp35-cp35m-linux_x86_64.whl
1.3 | 3.6 | CPU | https://github.com/mind/wheels/releases/download/tf1.3-cpu/tensorflow-1.3.0-cp36-cp36m-linux_x86_64.whl
1.3 | 2.7 | GPU | https://github.com/mind/wheels/releases/download/tf1.3-gpu/tensorflow-1.3.0-cp27-cp27mu-linux_x86_64.whl
1.3 | 3.5 | GPU | https://github.com/mind/wheels/releases/download/tf1.3-gpu/tensorflow-1.3.0-cp35-cp35m-linux_x86_64.whl
1.3 | 3.6 | GPU | https://github.com/mind/wheels/releases/download/tf1.3-gpu/tensorflow-1.3.0-cp36-cp36m-linux_x86_64.whl
1.3.1 | 2.7 | CPU | https://github.com/mind/wheels/releases/download/tf1.3.1-cpu/tensorflow-1.3.1-cp27-cp27mu-linux_x86_64.whl
1.3.1 | 3.5 | CPU | https://github.com/mind/wheels/releases/download/tf1.3.1-cpu/tensorflow-1.3.1-cp35-cp35m-linux_x86_64.whl
1.3.1 | 3.6 | CPU | https://github.com/mind/wheels/releases/download/tf1.3.1-cpu/tensorflow-1.3.1-cp36-cp36m-linux_x86_64.whl
1.3.1 | 2.7 | GPU | https://github.com/mind/wheels/releases/download/tf1.3.1-gpu/tensorflow-1.3.1-cp27-cp27mu-linux_x86_64.whl
1.3.1 | 3.5 | GPU | https://github.com/mind/wheels/releases/download/tf1.3.1-gpu/tensorflow-1.3.1-cp35-cp35m-linux_x86_64.whl
1.3.1 | 3.6 | GPU | https://github.com/mind/wheels/releases/download/tf1.3.1-gpu/tensorflow-1.3.1-cp36-cp36m-linux_x86_64.whl
1.4 | 2.7 | CPU | https://github.com/mind/wheels/releases/download/tf1.4-cpu/tensorflow-1.4.0-cp27-cp27mu-linux_x86_64.whl
1.4 | 3.5 | CPU | https://github.com/mind/wheels/releases/download/tf1.4-cpu/tensorflow-1.4.0-cp35-cp35m-linux_x86_64.whl
1.4 | 3.6 | CPU | https://github.com/mind/wheels/releases/download/tf1.4-cpu/tensorflow-1.4.0-cp36-cp36m-linux_x86_64.whl

## Help!

This section contains tips for debugging your setup. Seriously though, try [TinyMind](https://www.tinymind.com) out and you will never need to waste time debugging again. We also have [Docker images](https://hub.docker.com/r/tinymind/tensorflow/) that you can use on your own machines. If this section doesn't solve your problem, be sure to file an issue.

### CUDA

Different TensorFlow versions support/require different CUDA versions:

TF Version | CUDA | cuDNN
-----------|------|------
1.1, 1.2 | 8.0 | 5.1
1.2.1-1.3.1 | 8.0 | 6.0
1.4 | 9.0 | 7.0

In particular, TensorFlow < 1.4 doesn't work with CUDA 9, the current version. Instead of `sudo apt-get install cuda`, do `sudo apt-get install cuda-8-0`.

```sh
# Install CUDA 8
curl -O http://developer.download.nvidia.com/compute/cuda/repos/ubuntu1604/x86_64/cuda-repo-ubuntu1604_8.0.61-1_amd64.deb
sudo dpkg -i cuda-repo-ubuntu1604_8.0.61-1_amd64.deb
sudo apt-get update
sudo apt-get install cuda-8-0

# Install CUDA 9
curl -O http://developer.download.nvidia.com/compute/cuda/repos/ubuntu1604/x86_64/cuda-repo-ubuntu1604_9.0.176-1_amd64.deb
sudo dpkg -i cuda-repo-ubuntu1604_9.0.176-1_amd64.deb
sudo apt-get update
sudo apt-get install cuda
```

Make sure that CUDA-related environment variables are set properly:

```sh
echo 'export CUDA_HOME=/usr/local/cuda' >> ~/.bashrc
echo 'export PATH=$PATH:$CUDA_HOME/bin' >> ~/.bashrc
echo 'export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CUDA_HOME/lib64' >> ~/.bashrc
. ~/.bashrc
```

[Download the correct cuDNN](https://developer.nvidia.com/cudnn) and install it as follows:

```sh
# The cuDNN tar file.
tar xzvf cudnn-9.0-linux-x64-v7.0.tgz
sudo cp cuda/lib64/* /usr/local/cuda/lib64/
sudo cp cuda/include/cudnn.h /usr/local/cuda/include/
```

Missing `libcupti` library? Install it and add it to your `PATH`.

```sh
sudo apt-get install libcupti-dev
echo 'export LD_LIBRARY_PATH=/usr/local/cuda/extras/CUPTI/lib64:$LD_LIBRARY_PATH' >> ~/.bashrc
```

### MPI

Using a wheel with MPI support? Be sure to run `sudo apt-get install mpich`.
