# Wheels

Custom builds for TensorFlow with platform optimizations, including SSE, AVX and FMA.

These wheels are built for use on [TinyMind](https://www.tinymind.ai), the cloud machine learning platform. If you want to install them on your own Linux box, you can do so with:

```sh
pip --no-cache-dir install https://github.com/mind/wheels/releases/download/{RELEASE}/{WHEEL}
```

The wheels can be found in the [releases page](https://github.com/mind/wheels/releases).

## TensorFlow

Please note that your machine needs to have a relatively new Intel CPU (and nvidia GPU if you use the GPU version) to be compatible with the wheels below. TensorFlow versions of 1.2.1 and above use CuDNN 6, whereas 1.1 and 1.2 use CuDNN 5.1.

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
1.3 | 2.7 | CPU | https://github.com/mind/wheels/releases/download/tf1.3-cpu/tensorflow-1.3-cp27-cp27mu-linux_x86_64.whl
1.3 | 3.5 | CPU | https://github.com/mind/wheels/releases/download/tf1.3-cpu/tensorflow-1.3-cp35-cp35m-linux_x86_64.whl
1.3 | 3.6 | CPU | https://github.com/mind/wheels/releases/download/tf1.3-cpu/tensorflow-1.3-cp36-cp36m-linux_x86_64.whl
1.3 | 2.7 | GPU | https://github.com/mind/wheels/releases/download/tf1.3-gpu/tensorflow-1.3-cp27-cp27mu-linux_x86_64.whl
1.3 | 3.5 | GPU | https://github.com/mind/wheels/releases/download/tf1.3-gpu/tensorflow-1.3-cp35-cp35m-linux_x86_64.whl
1.3 | 3.6 | GPU | https://github.com/mind/wheels/releases/download/tf1.3-gpu/tensorflow-1.3-cp36-cp36m-linux_x86_64.whl
