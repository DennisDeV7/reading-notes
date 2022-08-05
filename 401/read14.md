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

## Class

you can and often want to use matplotlib, but sometimes you will want to use Seaborn

```py
def plot_some_lines():
  x1 = [10,20,5,40,8]
  x2 = [30,43,9,7,20]

  plt.plot(x1, label="Group Spam")
  plt.plot(x2, label="Group Eggs")
  plt.legend()

plot_some_lines()
```

Lets try Seaborn

```py
import seaborn as sns

sns.set()
plot_some_lines()
```

Built in Seaborn data set functions

```py
sns.load_dataset? # gives information on load_dataset
sns.get_dataset_names() # gives a list of data set names available through the internet
```

```py
mpg_df = sns.load_dataset("mpg")
mpg_df.head()
```

info on four cylinder cars

```py
four_cylinders = mpg_df[mpg_df.cylinders == 4]
four_cylinders.head()
```

Compare mpg for 4 cylinder vehicles in different countries

```py
four_cylinders = mpg_df[mpg_df.cylinders == 4]
by_origin = four_cylinders.groupby("origin", as_index=False)
mpg_by_origin = by_origin.mpg.mean()
sns.barplot(x="origin", y="mpg", data=mpg_by_origin)
print() # can sometimes clean it up if it prints a weird statement
```

```py
sns.countplot(data=mpg_df, x="cylinders")
print()
```

```py
avg_mpg = mpg_df.groupby("model_year", as_index=False).mpg.mean()
sns.relplot(x="model_year", y="mpg", data=avg_mpg)
```