# COBOL OCCURS Clause Without Index Bug

This repository demonstrates a common error in COBOL programs involving the `OCCURS` clause without proper indexing.  The bug occurs when attempting to access or modify elements within an array defined using `OCCURS` without providing an index. This can lead to unexpected behavior, data corruption, or program crashes.

## Bug Description
The primary issue lies in the improper use of the `OCCURS` clause within the `WS-DATA-AREA`.  Accessing `WS-ARRAY` without a valid index will cause unpredictable results because COBOL needs an index to know where to access or modify the elements in the array.

## Solution
The solution involves correctly using subscripts (indices) when accessing or manipulating elements within the `WS-ARRAY`.  The updated code provides a clear example of how to effectively use an index to avoid this problem. 