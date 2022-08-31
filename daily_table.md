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

WEEK 3 AUG 16 - AUG 23
|#| PATTERN     |       QUESTION     | Python CODE LINK  | NOTES |
|------:| ------------- |:-------------:| -----:|------:|
|1| TREE BREADTH FIRST TRAVERSAL| Binary Tree Level Order Traversal (easy)| https://leetcode.com/problems/binary-tree-level-order-traversal/submissions/| A breadth first search can be done using a queue easily|
|2|TREE BREADTH FIRST SEARCH| Zigzag Traversal (medium) | https://leetcode.com/problems/binary-tree-zigzag-level-order-traversal/submissions/| Same method as previous; Smart way is not change order of the queue; just add from left to right each time and while adding to result based on direction % 2 == 0 or not change order using a very crafty a[::-1] for reverse or a[::1] for normal|
|3|TREE DEPTH FIRST TRAVERSAL| Sum of Path Numbers (medium) | https://leetcode.com/problems/sum-root-to-leaf-numbers/submissions/|Classic dfs problem - boils down to what the helper returns; for converting nodes to integrer, *10 each num and add to current value|
|4|TREE DEPTH FIRST TRAVERSAL| Invert Binary Tree (Easy) |https://leetcode.com/problems/invert-binary-tree/submissions/ |Very easy dfs problem, main function is the recursive helper, at each node invert children and run fn. on left and right children|


WEEK 4 - Aug 24 - Aug31
|#| PATTERN     |       QUESTION     | Python CODE LINK  | NOTES |
|------:| ------------- |:-------------:| -----:|------:|
|1| DYNAMIC PROGRAMMING | Unique Binary Search Trees (medium) |https://leetcode.com/problems/unique-binary-search-trees/submissions/ | 1. The number of trees possible for a particular number of n remains the same regardless of the elements making up n nodes 2. For any node as the root, the number of possibe trees to make up a search tree is number of possible trees on left * number of possible trees on right 3. Store all possible trees for each node to recall in each iteration|
|2|TREE DEPTH FIRST SEARCH| Validate Binary Search Tree (Medium) |https://leetcode.com/problems/validate-binary-search-tree/submissions/ | Initial error: Not thinking that entire subtrees need to obey the binary search tree conditions. Starting with -inf anf + inf tow bounds can be used to check if a node value satiisfies binary search tree conditions|
|3|GRAPHS| Clone Graph (Medium)|https://leetcode.com/problems/clone-graph/submissions/|Graph problems require a hashmap and a traversal like dfs or bfs to visit a node; Create a hashmap to make clones of the graph; If node already there in hasmap return the clone to be appended to the neigbours of another node; Append neighbours from either the hasmap or add to hashmap and return with recursion DFS|
|4|GRAPHS|Tasks Scheduling (medium)|||
|5|K ELEMENTS| Top 'K' frequent Numbers (Medium)|https://leetcode.com/problems/top-k-frequent-elements/submissions/ | BUCKET SORT - Create a list of lists where each of the lists corresponds to all numbers with the same count and get top k ; alternatively use a max heap and pop two top k elements in log n time|
|6|K ELEMENTS / SLIDING WINDOW/ 2 POINTERS| Top 'K' Closest elements (HARD) |https://leetcode.com/problems/find-k-closest-elements/submissions/| Complicated algorithm - Unique; Define two pointers from begining to upto k to define window; Define a midpoint using the binary search technique in the window; Move left and right pointers based on the value among left and right ends close to x and return k elements from left pointer - HARD PROBLEM   
