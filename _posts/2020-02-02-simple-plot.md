---
layout: post
title: "Carregando um notebook Jupyter"
author: "Helon D. M. Braz"
date: 2020-02-02 14:00:00 -0300
categories: [programacao]
---

```python
%matplotlib inline
```

# Simple Plot

Create a simple plot.

```python
import matplotlib
import matplotlib.pyplot as plt
import numpy as np

# Data for plotting
t = np.arange(0.0, 2.0, 0.01)
s = 1 + np.sin(2 * np.pi * t)

fig, ax = plt.subplots()
ax.plot(t, s)

ax.set(xlabel='time (s)', ylabel='voltage (mV)',
       title='About as simple as it gets, folks')
ax.grid()

fig.savefig("test.png")
plt.show()
```

![png]({{ "/assets/images/output_2_0.png" }})

------------

## References

The use of the following functions and methods is shown in this example:

```python
matplotlib.axes.Axes.plot
matplotlib.pyplot.plot
matplotlib.pyplot.subplots
matplotlib.figure.Figure.savefig
```
<function matplotlib.figure.Figure.savefig(self, fname, *, transparent=None, **kwargs)>
