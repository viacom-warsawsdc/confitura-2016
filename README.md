# [Viacom Tech Confitura 2016 site](http://tech.viacom.com/warsawsdc/confitura2016/)

### General hints:

* input data will be provided via standard input
* output should be printed to the standard output
* specific in/out formats is defined in each task
* All error messages should be printed to the standard output in a following format:
```
 Error: {message}
``` 
 where `{message}` should be substituted with detailed information on what went wrong 
* If you want, you can add README to the root directory of each solution describing approach, assumptions or the way to execute your code

## 1. Layered tree
The input is a list of integers in random order.
The goal of this task is to create `layered` sorted binary tree.
Sorting order is defined as following:

* lower values should be placed in the upper part of the tree
* odd layers of the tree should be sorted in natural order
* even layers should be sorted in the reverse order

Missing nodes should be represented as `_` in the output.

### Example input and output
Input consists of 1 row of comma separated integers.

Example #1:
```
5,4,3,2,1
```

should result in a following tree:
```
    1
   / \
  3   2
 / \
4   5
```

And eventual output:
```
1
3,2
4,5,_,_
```

Example #2:
```
9,8,7,6,5,4,3,2,1
```

should result in a following tree:
```
     1
    / \
   /   \
  3     2
 / \   /  \
4   5 6    7
          / \
         9   8
```

And eventual output:
```
1
3,2
4,5,6,7
_,_,_,_,_,_9,8
```


## 2.  Prime tables
The input is a M x N table of numbers >= 0.

You have to find the number of subtables with dimensions at least 2x2 which satisfy following condition:

* the sum of all numbers in the subtable is a prime number

### Example input and output
Each line is a comma separated row with numbers.

For example input:
```
1,1,1,1
1,2,1,1
1,1,1,1
```
The result should be:
```
11
```

## 3. Lazy hiker

The input is a M x N table of numbers >= 0 and represents a map of an island, where value at cell (x, y) represents it's height.

The hiker begins his expedition in the top left corner (0,0) and heads towards to bottom right (M-1, N-1) and has 4 options of movement:

* L - left
* R - right
* U - up
* D - down

Our hiker is a bit lazy, so the goal is to find the most convenient path:
* the path should have the lowest sum of ascents
* if 2 or more paths have the same score, the one with the lowest sum of descents is more convenient

Hint: There might be more than one result.

### Example input and output
Every line contains one comma separated row of the map

For given input:
```
1,1,1,1 
1,2,3,1 
1,5,3,1 
1,1,1,1
```

Expected result is:
```
RRRDDD
DDDRRR
```

And for following input:
```
1,9,9,9
1,1,1,9
9,9,1,9
9,1,1,9
9,1,9,9
9,1,1,1
```
The expected result is:
```
DRRDDLDDRR
```

---
You can check contest bye-laws [here](http://tech.viacom.com/warsawsdc/confitura2016/Regulamin_konkurs_Viacom_programmer_adventure_2016.pdf).

Check out our Confitura 2016 site [here](http://tech.viacom.com/warsawsdc/confitura2016/)

We are hiring! Visit our [career site](http://tech.viacom.com/careers/).
