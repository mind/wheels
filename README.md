# Wheels

Custom builds for TensorFlow with platform optimizations, including SSE, AVX and FMA.

These wheels are built for use on [TinyMind](https://www.tinymind.ai), the cloud machine learning platform. If you want to install them on your own Linux box, you can do so with:

```sh
pip --no-cache-dir install https://raw.githubusercontent.com/mind/wheels/master/tensorflow/{YOUR_DESIRED_WHEEL}
```

Please note that your machine needs to have a relatively new CPU (or nVidia GPU if you use the GPU version) to be compatible with the wheels. TensorFlow versions of 1.2.1 and above use CuDNN 6, whereas 1.1 and 1.2 use CuDNN 5.1.
