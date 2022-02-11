## Binary Search
When the list is sorted we can use the binary search technique to find items on the list. 

In this procedure, the entire list is divided into two sub-lists. If the item is found in the middle position, it returns the location, otherwise jumps to either left or right sub-list and do the same process again until finding the item or exceed the range.

### The complexity of Binary Search Technique
> Time Complexity: O(1) for the best case. O(log2 n) for average or worst case.

>Space Complexity: O(1)


Binary Search Tree, is a node-based binary tree data structure which has the following properties:

 - The left subtree of a node contains only nodes with keys lesser than the node’s key.
 - The right subtree of a node contains only nodes with keys greater than the node’s key.
 - The left and right subtree each must also be a binary search tree. There must be no duplicate nodes.

#### Problem Statement
> Given a Array find the element 2,3,4,5,6 in the Array { 2,3,4,5,6,6 }
```java
import java.util.Arrays;

public class BinarySearch {
    public static void main(String[] args) {
        int[] array = {2, 3, 4, 5, 6, 6};
        System.out.println(binarySearch(array, 2));
        System.out.println(binarySearch(array, 3));
        System.out.println(binarySearch(array, 4));
        System.out.println(binarySearch(array, 5));
        System.out.println(binarySearch(array, 6));
    }

    public static int binarySearch(int[] arr, int elem) {
        System.out.println(Arrays.toString(arr));
        int result = -1;
        int start = 0;
        int end = arr.length - 1;

        while (start <= end) {
            int mid = (start + end) / 2;
            if (arr[mid] == elem) {
                return mid;
            }
            if (arr[mid] > elem) {
                end = mid - 1;
            }

            if (arr[mid] < elem) {
                start = mid + 1;
            }
        }
        return result;
    }
}

```
