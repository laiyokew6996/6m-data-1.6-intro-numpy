## **Package vs Module**

* **Module** \- single Python file (`.py`) containing code (functions, classes, variables) you can reuse. `numpy` itself is built out of many modules.

* **Package** \- folder of related modules bundled together, distributed and installed as one unit (e.g. via `pip install numpy`). `numpy` is a package.

  ```python
  import numpy as np       # importing the numpy package
  ```

  When you write `np.array(...)`, `np` is just an alias pointing at the numpy package - everything you call through it (functions, methods, attributes below) lives inside that package.

## **Function vs Method vs Attribute**

New to Python? These three terms look similar but mean different things:

* **Function** \- standalone tool, called by itself or `module.name()`. Pass data into it directly.
  ```python
  len(my_array)
  np.sum(my_array)
  ```

* **Method** \- function that belongs to an object. Called with a dot e.g. `object.name()`, no need to pass the object itself in (object already "owns" it). Always has `()`, even if empty.
  ```python
  my_array.sum()
  my_array.reshape(2, 3)
  ```

* **Attribute** \- piece of data stored on an object, not an action. object.name, No `()` \- you're not calling anything, just reading a value.
  ```python
  my_array.shape
  my_array.dtype
  ```

**Quick check:** see `()` after the dot → method (does something). No `()` → attribute (describes something).

## **Recommended Reading**

* [Interactive HTML to explain NumPy Arrays](https://su-ntu-ctp.github.io/6m-data-1.6-intro-numpy/) \- A great interactive resource to understand NumPy concepts.

* [NumPy Illustrated: A Visual Guide](https://medium.com/better-programming/numpy-illustrated-the-visual-guide-to-numpy-3b1d4976de1d) \- Excellent for visual learners.  
* [Official NumPy Quickstart](https://numpy.org/doc/stable/user/quickstart.html)

**Next Lesson:** 1.7 Introduction to Pandas. We will take these NumPy arrays and turn them into powerful DataFrames with labels\!
