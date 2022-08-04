# Data Visualization

## Matplotlib

[rougier Github matplotlib tutorial](https://github.com/rougier/matplotlib-tutorial)

matplot lib is a library that enables 2d graphics for analyzing data.

### IPython

Another good library is ipython. Ipython is an enhanced interactive shell that has a lot of useful features and allows interactive matplotlib sessions.

### pyplot

Pyplot provides a interface to matplotlib so that you can interact with plots created by matplotlib

Useful ways to manipulate a plot

- plt.figure(figsize=(10, 6), dpi=80): changes the size of the graph
- plt.plot(X, data_set, color="blue", linewidth=2.5, linestyle="-"): changes the color of the line that represents the data
- plt.xlim(X.min()*1.1, X.max()*1.1): sets limits so the plot is displayed with some white space, default is to match the window to the size of the data set
- plt.xticks( [-np.pi, -np.pi/2, 0, np.pi/2, np.pi]): setting the ticks on the axis
- plt.yticks([-1, 0, +1]): setting the ticks on the y-axis
- plt.xticks([-np.pi, -np.pi/2, 0, np.pi/2, np.pi],\
       [r'$-\pi$', r'$-\pi/2$', r'$0$', r'$+\pi/2$', r'$+\pi$']): sets the label for the ticks
- plt.yticks([-1, 0, +1],\
       [r'$-1$', r'$0$', r'$+1$']): sets the label for the ticks

Adding a legend

 ```py
plt.plot(X, C, color="blue", linewidth=2.5, linestyle="-", label="cosine")
plt.plot(X, S, color="red",  linewidth=2.5, linestyle="-", label="sine")

plt.legend(loc='upper left', frameon=False)
```

Annotating an Axis

```py
t = 2*np.pi/3
plt.plot([t,t],[0,np.cos(t)], color ='blue', linewidth=1.5, linestyle="--")
plt.scatter([t,],[np.cos(t),], 50, color ='blue')

plt.annotate(r'$\sin(\frac{2\pi}{3})=\frac{\sqrt{3}}{2}$',
             xy=(t, np.sin(t)), xycoords='data',
             xytext=(+10, +30), textcoords='offset points', fontsize=16,
             arrowprops=dict(arrowstyle="->", connectionstyle="arc3,rad=.2"))

plt.plot([t,t],[0,np.sin(t)], color ='red', linewidth=1.5, linestyle="--")
plt.scatter([t,],[np.sin(t),], 50, color ='red')

plt.annotate(r'$\cos(\frac{2\pi}{3})=-\frac{1}{2}$',
             xy=(t, np.cos(t)), xycoords='data',
             xytext=(-90, -50), textcoords='offset points', fontsize=16,
             arrowprops=dict(arrowstyle="->", connectionstyle="arc3,rad=.2"))
```

## Things I want to know more about

Everything I can do with these data related libraries. Jobs available for this area of programming.