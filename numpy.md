
# Table of Contents

1.  [Built-in methods to create arrays](#org1ba049c)
    1.  [`array`](#org8a56408)
    2.  [`arange`](#org3a8d816)
    3.  [`zeros`, `ones`](#org5902444)
    4.  [`linspace`](#org418d9da)
    5.  [`eye`](#org325eeb9)
2.  [Random](#org5f8e225)
    1.  [`seed`](#org2c26a0c)
    2.  [`rand`](#org628072c)
    3.  [`randn`](#org77f5f31)
    4.  [`randint`](#orgc0b1811)
3.  [Array attributes and methods](#org77195c7)
    1.  [`reshape`](#org1266411)
    2.  [`min`, `max`, `argmin`, `argmax`](#org8593992)
    3.  [`shape`, `(rows, columns, ...)`](#orge080a47)
    4.  [`ndim`](#org29470af)
    5.  [`dtype`](#org9422db8)
    6.  [`size`](#org75f2695)
    7.  [`itemsize`](#orge433bbd)
4.  [Indexing and slicing](#org1aaaf48)
    1.  [Slicing 1-D](#org88ed2ef)
    2.  [`copy`](#org23327fd)
    3.  [Broadcasting](#org64adf85)
    4.  [Slicing 2-D](#orge6f337b)
5.  [Conditional selection](#orgd91c216)
6.  [Operations](#org0af7154)
    1.  [`+`, `-`, `/`, `*`](#org4ec5a77)
7.  [Data types](#org789f7ed)
    1.  [Numpy data types](#orgae9e9bf)
    2.  [Constructing with data type](#org4255104)
    3.  [Structured arrays](#org97f64ba)
    4.  [Endiannes](#org120e0b2)



<a id="org1ba049c"></a>

# Built-in methods to create arrays


<a id="org8a56408"></a>

## `array`

    np.array([[1,2,3],[4,5,6],[7,8,9]])

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">1</td>
<td class="org-right">2</td>
<td class="org-right">3</td>
</tr>


<tr>
<td class="org-right">4</td>
<td class="org-right">5</td>
<td class="org-right">6</td>
</tr>


<tr>
<td class="org-right">7</td>
<td class="org-right">8</td>
<td class="org-right">9</td>
</tr>
</tbody>
</table>


<a id="org3a8d816"></a>

## `arange`

    np.arange(0, 11, 2)

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0</td>
<td class="org-right">2</td>
<td class="org-right">4</td>
<td class="org-right">6</td>
<td class="org-right">8</td>
<td class="org-right">10</td>
</tr>
</tbody>
</table>


<a id="org5902444"></a>

## `zeros`, `ones`

    np.zeros((5, 5))

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
</tr>


<tr>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
</tr>


<tr>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
</tr>


<tr>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
</tr>


<tr>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
</tr>
</tbody>
</table>


<a id="org418d9da"></a>

## `linspace`

Return `n` evenly spaced numbers over `[a, b]` (both inclusive).

    np.linspace(0, 5, 11)

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0</td>
<td class="org-right">0.5</td>
<td class="org-right">1</td>
<td class="org-right">1.5</td>
<td class="org-right">2</td>
<td class="org-right">2.5</td>
<td class="org-right">3</td>
<td class="org-right">3.5</td>
<td class="org-right">4</td>
<td class="org-right">4.5</td>
<td class="org-right">5</td>
</tr>
</tbody>
</table>


<a id="org325eeb9"></a>

## `eye`

Creates an identity matrix.

    np.eye(4)

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">1</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
</tr>


<tr>
<td class="org-right">0</td>
<td class="org-right">1</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
</tr>


<tr>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">1</td>
<td class="org-right">0</td>
</tr>


<tr>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">0</td>
<td class="org-right">1</td>
</tr>
</tbody>
</table>


<a id="org5f8e225"></a>

# Random


<a id="org2c26a0c"></a>

## `seed`

    np.random.seed(42)
    np.random.rand(4)

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0.37454012</td>
<td class="org-right">0.95071431</td>
<td class="org-right">0.73199394</td>
<td class="org-right">0.59865848</td>
</tr>
</tbody>
</table>


<a id="org628072c"></a>

## `rand`

Creates an array of the given shape populated with random samples from a
**uniform distribution** over [0, 1].

    np.random.rand(5,5)

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0.15601864</td>
<td class="org-right">0.15599452</td>
<td class="org-right">0.05808361</td>
<td class="org-right">0.86617615</td>
<td class="org-right">0.60111501</td>
</tr>


<tr>
<td class="org-right">0.70807258</td>
<td class="org-right">0.02058449</td>
<td class="org-right">0.96990985</td>
<td class="org-right">0.83244264</td>
<td class="org-right">0.21233911</td>
</tr>


<tr>
<td class="org-right">0.18182497</td>
<td class="org-right">0.18340451</td>
<td class="org-right">0.30424224</td>
<td class="org-right">0.52475643</td>
<td class="org-right">0.43194502</td>
</tr>


<tr>
<td class="org-right">0.29122914</td>
<td class="org-right">0.61185289</td>
<td class="org-right">0.13949386</td>
<td class="org-right">0.29214465</td>
<td class="org-right">0.36636184</td>
</tr>


<tr>
<td class="org-right">0.45606998</td>
<td class="org-right">0.78517596</td>
<td class="org-right">0.19967378</td>
<td class="org-right">0.51423444</td>
<td class="org-right">0.59241457</td>
</tr>
</tbody>
</table>


<a id="org77f5f31"></a>

## `randn`

Uses the **standard distribution** (σ = 1) to populate the array.

    np.random.randn(2)

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0.12221917</td>
<td class="org-right">-0.51543566</td>
</tr>
</tbody>
</table>


<a id="orgc0b1811"></a>

## `randint`

Returns random integers from `low` (inclusive) to `high` (exclusive).

    np.random.randint(0, 100)

    20

    np.random.randint(0, 10, 9)

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">8</td>
<td class="org-right">6</td>
<td class="org-right">1</td>
<td class="org-right">3</td>
<td class="org-right">8</td>
<td class="org-right">1</td>
<td class="org-right">9</td>
<td class="org-right">8</td>
<td class="org-right">9</td>
</tr>
</tbody>
</table>


<a id="org77195c7"></a>

# Array attributes and methods


<a id="org1266411"></a>

## `reshape`

(`rows`, `columns`)

    np.arange(0, 25).reshape(5, 5)

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0</td>
<td class="org-right">1</td>
<td class="org-right">2</td>
<td class="org-right">3</td>
<td class="org-right">4</td>
</tr>


<tr>
<td class="org-right">5</td>
<td class="org-right">6</td>
<td class="org-right">7</td>
<td class="org-right">8</td>
<td class="org-right">9</td>
</tr>


<tr>
<td class="org-right">10</td>
<td class="org-right">11</td>
<td class="org-right">12</td>
<td class="org-right">13</td>
<td class="org-right">14</td>
</tr>


<tr>
<td class="org-right">15</td>
<td class="org-right">16</td>
<td class="org-right">17</td>
<td class="org-right">18</td>
<td class="org-right">19</td>
</tr>


<tr>
<td class="org-right">20</td>
<td class="org-right">21</td>
<td class="org-right">22</td>
<td class="org-right">23</td>
<td class="org-right">24</td>
</tr>
</tbody>
</table>


<a id="org8593992"></a>

## `min`, `max`, `argmin`, `argmax`

    arr = np.random.randint(0, 100, 10)
    arr

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">52</td>
<td class="org-right">1</td>
<td class="org-right">83</td>
<td class="org-right">91</td>
<td class="org-right">59</td>
<td class="org-right">70</td>
<td class="org-right">43</td>
<td class="org-right">7</td>
<td class="org-right">46</td>
<td class="org-right">34</td>
</tr>
</tbody>
</table>

Get maximum value.

    arr.max()

    91

Get minimum value.

    arr.min()

    1

Get index of the maximum value.

    arr.argmax()

    3

Get index of the minimum value.

    arr.argmin()

    1


<a id="orge080a47"></a>

## `shape`, `(rows, columns, ...)`

Each element in a numpy array is a row. However, when
displayed, it is represented horizontally. It is better to think of it as
vertical.

    np.arange(0, 25).shape

    (25,)


<a id="org29470af"></a>

## `ndim`

    np.arange(0, 125).reshape(5, 5, 5).ndim

    3


<a id="org9422db8"></a>

## `dtype`

    arr = np.arange(0, 25, dtype='float16') # intx, uintx, floatx
    arr.dtype

    dtype('float16')


<a id="org75f2695"></a>

## `size`

Returns the length of the array.

    a = np.array([3, 1, 5, 2, 5, 1, 1, 5, 1, 4, 2, 1, 4, 5])
    a.size

    14


<a id="orge433bbd"></a>

## `itemsize`

Number of bytes that the underlying data type requires to store one element.

    np.array([1, 2, 3], dtype=np.uint64).itemsize

    8


<a id="org1aaaf48"></a>

# Indexing and slicing


<a id="org88ed2ef"></a>

## Slicing 1-D

Regular slicing methods used in lists apply. Slice will point to the original
arrays memory, which is not the case in regular lists.

    l1 = list(range(0, 10))
    l2 = l1[:5] # [:] operator shallow copies elements to a new array
    l1[1] = 100
    l2

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0</td>
<td class="org-right">1</td>
<td class="org-right">2</td>
<td class="org-right">3</td>
<td class="org-right">4</td>
</tr>
</tbody>
</table>

    a1 = np.arange(0, 10)
    a2 = a1[:5]
    a1[1] = 100
    a2

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0</td>
<td class="org-right">100</td>
<td class="org-right">2</td>
<td class="org-right">3</td>
<td class="org-right">4</td>
</tr>
</tbody>
</table>


<a id="org23327fd"></a>

## `copy`

    a1 = np.arange(0, 10)
    a2 = a1[:5].copy()
    a1[1] = 100
    a2

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0</td>
<td class="org-right">1</td>
<td class="org-right">2</td>
<td class="org-right">3</td>
<td class="org-right">4</td>
</tr>
</tbody>
</table>


<a id="org64adf85"></a>

## Broadcasting

    arr = np.arange(0, 10)
    arr[:5] = 100
    arr

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">100</td>
<td class="org-right">100</td>
<td class="org-right">100</td>
<td class="org-right">100</td>
<td class="org-right">100</td>
<td class="org-right">5</td>
<td class="org-right">6</td>
<td class="org-right">7</td>
<td class="org-right">8</td>
<td class="org-right">9</td>
</tr>
</tbody>
</table>


<a id="orge6f337b"></a>

## Slicing 2-D

Using `:` is important when slicing. It changes the shape of the output. Using
`:` keeps the shape.

    a = np.arange(0, 100, 5).reshape(4, 5)
    a

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0</td>
<td class="org-right">5</td>
<td class="org-right">10</td>
<td class="org-right">15</td>
<td class="org-right">20</td>
</tr>


<tr>
<td class="org-right">25</td>
<td class="org-right">30</td>
<td class="org-right">35</td>
<td class="org-right">40</td>
<td class="org-right">45</td>
</tr>


<tr>
<td class="org-right">50</td>
<td class="org-right">55</td>
<td class="org-right">60</td>
<td class="org-right">65</td>
<td class="org-right">70</td>
</tr>


<tr>
<td class="org-right">75</td>
<td class="org-right">80</td>
<td class="org-right">85</td>
<td class="org-right">90</td>
<td class="org-right">95</td>
</tr>
</tbody>
</table>

    a[1:3]

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">25</td>
<td class="org-right">30</td>
<td class="org-right">35</td>
<td class="org-right">40</td>
<td class="org-right">45</td>
</tr>


<tr>
<td class="org-right">50</td>
<td class="org-right">55</td>
<td class="org-right">60</td>
<td class="org-right">65</td>
<td class="org-right">70</td>
</tr>
</tbody>
</table>

    a[1:3,2:]

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">35</td>
<td class="org-right">40</td>
<td class="org-right">45</td>
</tr>


<tr>
<td class="org-right">60</td>
<td class="org-right">65</td>
<td class="org-right">70</td>
</tr>
</tbody>
</table>

    a[1:, 3:4] # != a[1:, 3]

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">40</td>
</tr>


<tr>
<td class="org-right">65</td>
</tr>


<tr>
<td class="org-right">90</td>
</tr>
</tbody>
</table>

    a[1:, 3]

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">40</td>
<td class="org-right">65</td>
<td class="org-right">90</td>
</tr>
</tbody>
</table>


<a id="orgd91c216"></a>

# Conditional selection

Includes a pointer to the original array.

    a = np.random.randint(0, 10, 20)
    a

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0</td>
<td class="org-right">3</td>
<td class="org-right">1</td>
<td class="org-right">7</td>
<td class="org-right">3</td>
<td class="org-right">1</td>
<td class="org-right">5</td>
<td class="org-right">5</td>
<td class="org-right">9</td>
<td class="org-right">3</td>
<td class="org-right">5</td>
<td class="org-right">1</td>
<td class="org-right">9</td>
<td class="org-right">1</td>
<td class="org-right">9</td>
<td class="org-right">3</td>
<td class="org-right">7</td>
<td class="org-right">6</td>
<td class="org-right">8</td>
<td class="org-right">7</td>
</tr>
</tbody>
</table>

    gt5 = a > 5
    a[gt5]

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">7</td>
<td class="org-right">9</td>
<td class="org-right">9</td>
<td class="org-right">9</td>
<td class="org-right">7</td>
<td class="org-right">6</td>
<td class="org-right">8</td>
<td class="org-right">7</td>
</tr>
</tbody>
</table>

    a[gt5] *= 10
    a

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-right">0</td>
<td class="org-right">3</td>
<td class="org-right">1</td>
<td class="org-right">70</td>
<td class="org-right">3</td>
<td class="org-right">1</td>
<td class="org-right">5</td>
<td class="org-right">5</td>
<td class="org-right">90</td>
<td class="org-right">3</td>
<td class="org-right">5</td>
<td class="org-right">1</td>
<td class="org-right">90</td>
<td class="org-right">1</td>
<td class="org-right">90</td>
<td class="org-right">3</td>
<td class="org-right">70</td>
<td class="org-right">60</td>
<td class="org-right">80</td>
<td class="org-right">70</td>
</tr>
</tbody>
</table>


<a id="org0af7154"></a>

# Operations


<a id="org4ec5a77"></a>

## `+`, `-`, `/`, `*`

Division by zero will not cause an error. Instead it will issue a warning.

    a = np.array([5, 7, 1, 0])
    print(a / 2)

    [2.5 3.5 0.5 0. ]

    print(a / a)

    [ 1.  1.  1. nan]

    print(a / 0)

    [inf inf inf nan]


<a id="org789f7ed"></a>

# Data types


<a id="orgae9e9bf"></a>

## Numpy data types

Here are some of the types that numpy supports. Consult the documentation for
more information.

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">Data type</th>
<th scope="col" class="org-left">Description</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left"><code>bool_</code>, <code>bool8</code></td>
<td class="org-left">Boolean</td>
</tr>


<tr>
<td class="org-left"><code>int_</code>, <code>intc</code>, <code>intp</code>, <code>int8</code>, <code>int16</code>, <code>int32</code>, <code>int64</code></td>
<td class="org-left">Integer types</td>
</tr>


<tr>
<td class="org-left"><code>uint</code>, <code>uintc</code>, <code>uintp</code>, <code>uint8</code>, <code>uint16</code>, <code>uint32</code>, <code>uint64</code></td>
<td class="org-left">Unsigned integer types</td>
</tr>


<tr>
<td class="org-left"><code>float_</code>, <code>float16</code>, <code>float32</code>, <code>float64</code></td>
<td class="org-left">Float types</td>
</tr>


<tr>
<td class="org-left"><code>complex_</code>, <code>complex64</code>, <code>complex128</code></td>
<td class="org-left">Complex types</td>
</tr>
</tbody>
</table>


<a id="org4255104"></a>

## Constructing with data type

    np.array([1, 2, 3, 4, 5], dtype=np.float16)

    array([1., 2., 3., 4., 5.], dtype=float16)


<a id="org97f64ba"></a>

## Structured arrays

Structured arrays are ndarrays whose datatype is a composition of simpler
datatypes organized as a sequence of named fields. They closely mimic C `struct` for low-level manipulation and interpretation of binary blobs.

1.  A list of tuples can be used to express the layout.
    `np.dtype([(fieldname, datatype, shape), ...])` where `shape` is optional.
2.  A string of comma-seperated dtype specifications.

    np.dtype('i8, f4, S3')

    dtype([('f0', '<i8'), ('f1', '<f4'), ('f2', 'S3')])

1.  A dictionary of field parameter arrays. This is the most flexible option.
    -   `names`, `formats` have to be specified and must be of the same length.
    -   `offsets` specifies the offset of each column from the start.
    -   `itemsize` specifies the total size of the structure. It must be able to
        contain the structure.

    # np.dtype({'names': ['col1', 'col2'], 'formats': ['i4', 'f4']})
    np.dtype({'names':   ['col1', 'col2'],
              'formats': ['i4',   'f4'],
              'offsets': [0,      4],
              'itemsize': 12})

    dtype({'names': ['col1', 'col2'], 'formats': ['<i4', '<f4'], 'offsets': [0, 4], 'itemsize': 12})

1.  A dictionary of field names.

    np.dtype({'col1': ('i1', 0), 'col2': ('f4', 1)})

    dtype([('col1', 'i1'), ('col2', '<f4')])

Here is a table called `population`.

<table id="org04b9cbc" border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<tbody>
<tr>
<td class="org-left">Netherlands</td>
<td class="org-right">393</td>
<td class="org-right">41526</td>
<td class="org-right">16928800</td>
</tr>


<tr>
<td class="org-left">Belgium</td>
<td class="org-right">337</td>
<td class="org-right">30510</td>
<td class="org-right">11007020</td>
</tr>


<tr>
<td class="org-left">United Kingdom</td>
<td class="org-right">256</td>
<td class="org-right">243610</td>
<td class="org-right">62262000</td>
</tr>


<tr>
<td class="org-left">Germany</td>
<td class="org-right">233</td>
<td class="org-right">357021</td>
<td class="org-right">81799600</td>
</tr>


<tr>
<td class="org-left">Liechtenstein</td>
<td class="org-right">205</td>
<td class="org-right">160</td>
<td class="org-right">32842</td>
</tr>


<tr>
<td class="org-left">Italy</td>
<td class="org-right">192</td>
<td class="org-right">301230</td>
<td class="org-right">59715625</td>
</tr>


<tr>
<td class="org-left">Switzerland</td>
<td class="org-right">177</td>
<td class="org-right">41290</td>
<td class="org-right">7301994</td>
</tr>


<tr>
<td class="org-left">Luxembourg</td>
<td class="org-right">173</td>
<td class="org-right">2586</td>
<td class="org-right">512000</td>
</tr>


<tr>
<td class="org-left">France</td>
<td class="org-right">111</td>
<td class="org-right">547030</td>
<td class="org-right">63601002</td>
</tr>


<tr>
<td class="org-left">Austria</td>
<td class="org-right">97</td>
<td class="org-right">83858</td>
<td class="org-right">8169929</td>
</tr>


<tr>
<td class="org-left">Greece</td>
<td class="org-right">81</td>
<td class="org-right">131940</td>
<td class="org-right">11606813</td>
</tr>


<tr>
<td class="org-left">Ireland</td>
<td class="org-right">65</td>
<td class="org-right">70280</td>
<td class="org-right">4581269</td>
</tr>


<tr>
<td class="org-left">Sweden</td>
<td class="org-right">20</td>
<td class="org-right">449964</td>
<td class="org-right">9515744</td>
</tr>


<tr>
<td class="org-left">Finland</td>
<td class="org-right">16</td>
<td class="org-right">338424</td>
<td class="org-right">5410233</td>
</tr>


<tr>
<td class="org-left">Norway</td>
<td class="org-right">13</td>
<td class="org-right">385252</td>
<td class="org-right">5033675</td>
</tr>
</tbody>
</table>

    pop_t = np.dtype([('country', 'U20'), ('density', '=i4'), ('area', '=i4'), ('population', '=i4')])
    np.array(population, dtype=pop_t)

    array([('Netherlands', 393,  41526, 16928800),
           ('Belgium', 337,  30510, 11007020),
           ('United Kingdom', 256, 243610, 62262000),
           ('Germany', 233, 357021, 81799600),
           ('Liechtenstein', 205,    160,    32842),
           ('Italy', 192, 301230, 59715625),
           ('Switzerland', 177,  41290,  7301994),
           ('Luxembourg', 173,   2586,   512000),
           ('France', 111, 547030, 63601002),
           ('Austria',  97,  83858,  8169929),
           ('Greece',  81, 131940, 11606813),
           ('Ireland',  65,  70280,  4581269),
           ('Sweden',  20, 449964,  9515744),
           ('Finland',  16, 338424,  5410233),
           ('Norway',  13, 385252,  5033675)],
          dtype=[('country', '<U20'), ('density', '<i4'), ('area', '<i4'), ('population', '<i4')])


<a id="org120e0b2"></a>

## Endiannes

-   `<i8` use little-endian. x86 architecture and some Arm chips use this
    format.
-   `>i8` use big-endian. This format should be used when transmitting data over
    a network.
-   `=i8` use native-endiannes of the system. It is system-dependant, so
    shouldn&rsquo;t be use accross systems.

