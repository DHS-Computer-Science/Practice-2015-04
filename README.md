# Practice 2015 - 04: Mapping the Universe

## Background
Thor is trying to plot all the realms on a map because he’s having trouble
keeping track of them. For maps like this, it is useful to give each region a
color so that they are easier to recognize. It is also best not to give adjacent
regions the same color, otherwise we couldn’t tell them apart. Thor is having
trouble designing his map because he doesn’t know how to color each realm. He
has given you a bunch of different maps he’s made, and he needs you to tell him
if each one is valid or not.

A valid coloring of a map is then one where no two adjacent regions have the
same color. Given a list of colored regions, and a list of borders between
regions, determine whether the coloring is valid or invalid.

## Description

### Input
The first line of the file will have an integer, n, which is the number of test
cases in this file.

Each test case will start with a line containing a single integer l. The next l
lines will each contain an integer r and string c, where r is an integer
representing a region and c is that region’s color. The region numbers will
start at zero and increase by one for each consecutive region. The region
numbers will always appear in properly sorted order (0 to l − 1). The map colors
will be alphanumeric strings, without any punctuation or spaces.

The following line will contain a single integer b. The next b lines will each
contain two integers a and b indicating that region a borders region
b (e.g. “1 2” indicates that region 1 borders region 2). These b lines
may appear in any order.

Region names and color names will only contain alphanumeric characters. However,
they are case sensitive, so ‘ASGARD’ is not the same region as ‘Asgard’.

There will be at most 200 regions, thus at most 40000 possible borders. The same
border may be listed multiple times for any one problem; additional listings
have no extra significance.

### Output
One line per test case containing valid if the coloring is valid, or invalid if
the coloring is invalid. Please pay attention to case in the output!

## Sample
### Input
```
2
3
0 red
1 orange
2 red
2
0 1
1 2
3
0 red
1 orange
2 red
3
0 1
1 2
0 2
```

### Output
```
valid
invalid
```
