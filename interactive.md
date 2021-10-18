## Getting interactive

In addition to building the book using the final state of the executed notebook, we can also enable interactive computation using a library called Thebe:

<!-- Configure and load Thebe !-->
<script type="text/x-thebe-config">
  {
    requestKernel: true,
    mountStatusWidget: true,
    mountActivateWidget: true,
    binderOptions: {
      repo: "binder-examples/requirements",
    },
    bootstrap: true
  }
</script>

<div class="thebe-activate"></div>
<div class="thebe-status"></div>

<script src="https://unpkg.com/thebe@latest/lib/index.js"></script>

<pre data-executable="true" data-language="python">
%matplotlib inline
import numpy as np
import matplotlib.pyplot as plt
x = np.linspace(0,10)
plt.plot(x, np.sin(x))
plt.plot(x, np.cos(x))
</pre>
