description: Returns which elements of x are NaN.

<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="tf.math.is_nan" />
<meta itemprop="path" content="Stable" />
</div>

# tf.math.is_nan

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">

</table>



Returns which elements of x are NaN.

<section class="expandable">
  <h4 class="showalways">View aliases</h4>
  <p>
<b>Compat aliases for migration</b>
<p>See
<a href="https://www.tensorflow.org/guide/migrate">Migration guide</a> for
more details.</p>
<p>`tf.compat.v1.debugging.is_nan`, `tf.compat.v1.is_nan`, `tf.compat.v1.math.is_nan`</p>
</p>
</section>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>tf.math.is_nan(
    x, name=None
)
</code></pre>



<!-- Placeholder for "Used in" -->



#### Example:



```python
x = tf.constant([5.0, np.nan, 6.8, np.nan, np.inf])
tf.math.is_nan(x) ==> [False, True, False, True, False]
```

<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Args</h2></th></tr>

<tr>
<td>
`x`
</td>
<td>
A `Tensor`. Must be one of the following types: `bfloat16`, `half`, `float32`, `float64`.
</td>
</tr><tr>
<td>
`name`
</td>
<td>
A name for the operation (optional).
</td>
</tr>
</table>



<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Returns</h2></th></tr>
<tr class="alt">
<td colspan="2">
A `Tensor` of type `bool`.
</td>
</tr>

</table>



#### Numpy Compatibility
Equivalent to np.isnan
