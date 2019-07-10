page_type: reference
<style>{% include "site-assets/css/style.css" %}</style>

<!-- DO NOT EDIT! Automatically generated file. -->

# tf.contrib.graph_editor.filter_ops

``` python
tf.contrib.graph_editor.filter_ops(
    ops,
    positive_filter
)
```



Defined in [`tensorflow/contrib/graph_editor/select.py`](https://github.com/tensorflow/tensorflow/blob/r1.13/tensorflow/contrib/graph_editor/select.py).

Get the ops passing the given filter.

#### Args:

* <b>`ops`</b>: an object convertible to a list of tf.Operation.
* <b>`positive_filter`</b>: a function deciding where to keep an operation or not.
    If True, all the operations are returned.

#### Returns:

A list of selected tf.Operation.

#### Raises:

* <b>`TypeError`</b>: if ops cannot be converted to a list of tf.Operation.