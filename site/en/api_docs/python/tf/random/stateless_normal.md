page_type: reference
<style>{% include "site-assets/css/style.css" %}</style>

<!-- DO NOT EDIT! Automatically generated file. -->

# tf.random.stateless_normal

### Aliases:

* `tf.contrib.stateless.stateless_random_normal`
* `tf.random.stateless_normal`

``` python
tf.random.stateless_normal(
    shape,
    seed,
    mean=0.0,
    stddev=1.0,
    dtype=tf.dtypes.float32,
    name=None
)
```



Defined in [`tensorflow/python/ops/stateless_random_ops.py`](https://github.com/tensorflow/tensorflow/blob/r1.13/tensorflow/python/ops/stateless_random_ops.py).

Outputs deterministic pseudorandom values from a normal distribution.

This is a stateless version of <a href="../../tf/random/normal"><code>tf.random_normal</code></a>: if run twice with the
same seeds, it will produce the same pseudorandom numbers.  The output is
consistent across multiple runs on the same hardware (and between CPU
and GPU), but may change between versions of TensorFlow or on non-CPU/GPU
hardware.

#### Args:

* <b>`shape`</b>: A 1-D integer Tensor or Python array. The shape of the output tensor.
* <b>`seed`</b>: A shape [2] integer Tensor of seeds to the random number generator.
* <b>`mean`</b>: A 0-D Tensor or Python value of type `dtype`. The mean of the normal
    distribution.
* <b>`stddev`</b>: A 0-D Tensor or Python value of type `dtype`. The standard deviation
    of the normal distribution.
* <b>`dtype`</b>: The type of the output.
* <b>`name`</b>: A name for the operation (optional).


#### Returns:

A tensor of the specified shape filled with random normal values.