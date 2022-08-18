WEEK 1 - July 25 - Aug 1


|#| PATTERN     |       QUESTION     | Python CODE LINK  | NOTES |
|------:| ------------- |:-------------:| -----:|------:|
|1| SLIDING WINDOWS     | Maximum Sum Subarray of Size K (easy) | https://leetcode.com/problems/sliding-window-maximum/submissions/  | Simple brute force solution but very time complex O(n*n-k); Faster soltuion can be obtained using a deque - decreasing queue|
|2|RECURSION or SLIDING WINDOWS|Longest Substring with At Least K Repeating Characters (Medium)|https://leetcode.com/problems/longest-substring-with-at-least-k-repeating-characters/submissions/| Brute force Solution is very expensive; solved using recursion, time complexity is still O(N^2) in recursion, there is a sliding window approach too with O(N)|
|3| TWO POINTERS        | Pair with Target Sum (easy)    | https://leetcode.com/problems/count-number-of-pairs-with-absolute-difference-k/submissions/   | Very simple splution using two pointers - Optimal solution ?|
|4|TWO POINTERS or HASH MAP| 2Sum (easy) | https://leetcode.com/problems/two-sum/submissions/ | Optimal solution can be obtained using a hash map - Traverse through the array, if num - target is in the hashmap return - O(N)|
|5|TWO POINTERS or HASH MAP| 2Sum II (Medium) | https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/submissions/ | Advantage of array being sorted is two pointers at opposite ends can be moved toward each depending on how close their sum is to target - Time Complexity O(N)|
|6| TWO POINTERS        | Triplet Sum to Zero (medium) | https://leetcode.com/problems/3sum/submissions/ | Main trick is to sort the array - this way for each number we can use TWO SUM II solved above and check for duplicates easily - O(NlogN) (sorting) + O(N^2) |



WEEK 2 AUG 2 - AUG 9

|#| PATTERN     |       QUESTION     | Python CODE LINK  | NOTES |
|------:| ------------- |:-------------:| -----:|------:|
|1| TREE DEPTH FIRST TRAVERSAL | Binary Tree Path Sum (easy) | https://leetcode.com/problems/path-sum/submissions/ | Depth first search on a binary tree can be done usin recursion; define a neew function to check if a node is a leaf or recursively do that left or right until a leaf is hit; Call this function recursively on root node |
|2|TREE DEPTH FIRST TRAVERSAL| All Paths for a Sum (medium) |https://leetcode.com/problems/path-sum-ii/submissions/ | Define a helper fucntion to check if its a leaf similar to prev, check if leaf val == target sum  - [remaining path node values], if not move left and right recursively while adding node value to list passed to next node - O(N) worst case |

AUG 10-15 Codeathon and thesis submissions 

WEEK 3 AUG 15 - AUG 22
|#| PATTERN     |       QUESTION     | Python CODE LINK  | NOTES |
|------:| ------------- |:-------------:| -----:|------:|
|1| FAST AND SLOW POINTERS | Happy Number (medium) | | |
|2| TREE BREADTH FIRST TRAVERSAL| Binary Tree Level Order Traversal (easy)| https://leetcode.com/problems/binary-tree-level-order-traversal/submissions/| A breadth first searchh can be done using a queue easily|
|3|TREE BREADTH FIRST SEARCH| Zigzag Traversal (medium) | https://leetcode.com/problems/binary-tree-zigzag-level-order-traversal/submissions/| Same method as previous; Smart way is not change order of the queue; just add from left to right each time and while adding to result based on direction % 2 == 0 or not change order using a very crafty a[::-1] for reverse or a[::1] for normal|
|4|TREE BREADTH FIRST SEARCH| Reverse Level Order Traversal (easy) | | |
|5|TREE DEPTH FIRST TRAVERSAL| Sum of Path Numbers (medium) | | |
|6|TREE BREADTH FIRST TRAVERSAL| Invert Binary Tree (Easy) | | |
|7|GRAPHS| Clone Graph (Medium)|||
|8| SLIDING WINDOWS| Longest Substring with K Distinct Characters (Medium)     |   |
