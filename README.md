# 594_HW1
Name: Lebin Hu
PennKey: hu28

Part1:
When the list is ArrayList, function A will run in time O(1) because arraylist can search variables directly with index; function B will run in time O(n) because to conduct remove(0), other remaining variables should be shifted at the same time. In this case, Lloyd is right.
When the list is LinkList, function A will run in time O(n) because to conduct lst.get(middle), the link list should be traversed; function B will run in time O(1) because in Java's d doublely linked circumstances, searhing and adjusting the first or the last element can be done directly. In this case, Alicia is right.

Part2:
1)
Snippet C:
Big O: O(n*m)
Big Ω: Ω(1)
Snippet D:
Big O: O(n*m)
Big Ω: Ω(n*m)
2)
When the target is at the beginning, Snippet C is faster, because Snippet C will exit from the loop when finding the target, while Snippet D will continue looping to the end.
When the target is at the end, Snippet D is faster because both of the two methods will check almost all of the elements and Snippet D has simpler logic(less comparison).
3)
Observation: when target is at the beginning, Snippet C runs always very fast; In other cases, first runs are slower than subsequent runs.
Consistency: it is not 100% consistent and will vary a little in specific running times.

Part3:
1）
I think LinkList will be faster because for the remove(0) operation, LinkList will run in time O(1) while ArrayList will run in time O(n).
2)
when the list size is small, two methods run equivalently fast; when the list size is large, LinkList version runs faster.
3)
Creation time will not affect the result because the difference mainly comes from "remove(0)" operation.
4)
Through this experience, I've learned that when choosing data structure, the key operation is a key factor. Since ticket processing system needs to remove(0) frequently, LinkedList with O(1) running time will be better. In ticket processing scenario, I will recommend LinkedList because of its efficiency in removal operation. ArrayList can be considered when frequent element searching is required(index can make this process faster). My experimental result matches the theoretical complexity when the dataset scale scale is large.

Part4:
1)
Big O Time: O(N*logN)
Big Ω Time: Ω(N*logN)
Big O Space: O(N)
Big Ω Space: Ω(N)
2）
Both implementations achieve O(N*logN) time complexity. The first one has O(N) space complexity, while the other one has O(N*logN). In actual runtime, the iterative version is faster because it avoids recursion overhead. I will recommend the first version because it is efficient for large dataset. But if the dataset is small and the code should be concise, then the recursion version can also be considered.
 


