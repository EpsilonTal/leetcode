Solution posted on:
* https://leetcode.com/problems/zigzag-conversion/discuss/549451/Java-Solution-O(n)-with-algorithm
* https://stackoverflow.com/questions/32915810/zigzag-conversion/60823333#60823333


The mathematic algorithm for zigzag is:

* originalDiff = numRows * 2 - 2;
* If -> 'currRow' equals First or last lines
	* use the originalDiff (numRows * 2 - 2)
* Else ->
	* For each new line:
		 * upperDiff += 2, 
		 * lowerDiff -=2
	
Examples:
```
### ### ### ### 
originalDiff = numRows * 2 - 2 
### ### ### ### 

numRows = 2 -> originalDiff = 2
PYAIHRN
APLSIIG

numRows  = 3 -> originalDiff = 4
P   A   H   N
A P L S I I G
Y   I   R

numRows = 4 -> originalDiff = 6
P    I    N
A  L S  I G
Y A  H R
P    I 

numRows = 5 -> originalDiff = 8
P    H   
A   SI   
Y  I R 
P L  I G  
A    N

```
