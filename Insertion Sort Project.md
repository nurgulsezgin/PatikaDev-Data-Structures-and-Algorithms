# Insertion Sort Project

[22,27,16,2,18,6] -> Insertion Sort


### 1. Write the stages of the above sequence according to the sort type.

#### First Pass:
<ul>
<li>The second element of the array is chosen as the starting element.
Here, 27 is greater than 22, thus both elements seems to be in ascending order, hence, no swapping will occur.
<br> 
    [22,27,<b>16</b>,2,18,6]
<br></li>
<li>Now, move to the next two elements which are 27, 16 and compare them..
27 is greater than 16, so swap them.
<br>
    [22,<b>16</b>,27,2,18,6]
<br> </li>
<li>After swapping, elements 22 and 16 are not sorted, thus swap again..
<br>
    [<b>16</b>,22,27,2,18,6]
<br></li>
</ul>

#### Second Pass:
In this step, it is time to look at the fourth element, the number 2. Since it is smaller than all of them, it swap again and again. Hence, it settles to the far left.\
[16,22,27,**2**,18,6]\
[16,22,**2**,27,18,6]\
[16,**2**,22,27,18,6]\
[**2**,16,22,27,18,6]

#### Third Pass:
Look at the fifth element which is 18. Now, 18 is smaller than 27 and 22. Hence, swap again twice.\
[2,16,22,**18**,27,6]\
[2,16,**18**,22,27,6]

#### Fourth Pass:
Look at the sixth element which is 6. Now, 6 is smaller than 27, 22, 18 and 16. Hence, swap again four times.\
[2,16,18,22,**6**,27]\
[2,16,18,**6**,22,27]\
[2,16,**6**,18,22,27]\
[2,**6**,16,18,22,27]

👋 Finally, the array is completely sorted.

### 2. Write the Big-O notation.

**Total process**  : 1 + (n-3) + (n-2) + (n-4) + (n-2) 
**Big-O notation** : [(n.(n+1))/2] - [(n-5) + (n-1)] +(n-2)]
--> **O(n²)**  

### 3. Time Complexity: Average case: The number we are looking for is in the middle, Worst case: The number we are looking for is at the end, Best case: The number we are looking for is at the beginning of the series.
  What case does the number 18 fall into after the array is sorted? Write.
Since the number of Time Complexity 18 is in the middle after the sorting it is included in the **Average case**.
### 4. Write the first 4 steps of [7,3,5,8,2,9,4,15.6] according to Insertion Sort.

**Steps:**
\
[7,3,5,8,2,9,4,15,6]

[3,7,5,8,2,9,4,15,6]\
[3,5,7,8,2,9,4,15,6]

[3,5,7,2,8,9,4,15,6]\
[3,5,2,7,8,9,4,15,6]\
[3,2,5,7,8,9,4,15,6]\
[2,3,5,7,8,9,4,15,6]

[2,3,5,7,8,4,9,15,6]\
[2,3,5,7,4,8,9,15,6]\
[2,3,5,4,7,8,9,15,6]\
[2,3,4,5,7,8,9,15,6]

[2,3,4,5,7,8,9,6,15]\
[2,3,4,5,7,8,6,9,15]\
[2,3,4,5,7,6,8,9,15]\
[2,3,4,5,6,7,8,9,15]
