# **Matplotlib tutorial:**

- matplotlib is probably the single most used Python package for 2D-graphics. It provides both a very quick way to visualize data from Python and publication-quality figures in many formats.

## **IPython**

- IPython is a Python shell with a rich history, auto-completion, and magics, enhanced interactive Python shell that has lots of interesting features including named inputs and outputs, access to shell commands, improved debugging and much more.

## **pyplot:**

- pyplot provides a convenient interface to the matplotlib object-oriented plotting library
- pyplot is a module that contains a large collection of functions for plotting.

     ![](https://miro.medium.com/max/9450/1*OAFEIg9w1XHyZk0xBud14A.png)

## get the data for the sine and cosine functions

```
        import numpy as np

        X = np.linspace(-np.pi, np.pi, 256, endpoint=True)
        C, S = np.cos(X), np.sin(X)
```

- X is now a NumPy array with 256 values ranging from -π to +π (included). C is the cosine (256 values) and S is the sine (256 values).

    ![](https://github.com/rougier/matplotlib-tutorial/raw/master/figures/exercice_1.png)

## Note

- Matplotlib comes with a set of default settings that allow customizing all kinds of properties. You can control the defaults of almost every property in matplotlib: figure size and dpi, line width, color and style, axes, axis and grid properties, text and font properties and so on. While matplotlib defaults are rather good in most cases, you may want to modify some properties for specific cases.

- EXAMPLE:

```
    plt.figure(figsize=(10,6), dpi=80)
    plt.plot(X, C, color="blue", linewidth=2.5, linestyle="-")
    plt.plot(X, S, color="red",  linewidth=2.5, linestyle="-")
```

## Animation

- For quite a long time, animation in matplotlib was not an easy task and was done mainly through clever hacks. However, things have started to change since version 1.1 and the introduction of tools for creating animation very intuitively, with the possibility to save them in all kind of formats (but don't expect to be able to run very complex animations at 60 fps though).

## Drip drop

A very simple rain effect can be obtained by having small growing rings randomly positioned over a figure. Of course, they won't grow forever since the wave is supposed to damp with time. To simulate that, we can use a more and more transparent color as the ring is growing, up to the point where it is no more visible. At this point, we remove the ring and create a new one.

recourse      | links
------------- | -------------
matplotlib-tutorial | [Link](https://github.com/rougier/matplotlib-tutorial)