1. A typical problem in our work at CardinalHire involves the processing of user input, which is often noisy, and often a string or array.

With the language of your choice, given two integer arrays (A and B), how would you sort and merge B into A as one sorted array?
```
I would sort the two arrays separately and then merge them. 
```

Note: You may assume that A has enough space to hold additional elements from B, and the number of elements initialized in A and B are M and N, respectively.

2. If, instead, the two arrays A and B are string arrays, with the language of your choice, how would you sort and merge B into A as one sorted array? Does your approach change?

Note: Same assumptions as above.

3. You are given a linked list and a value: k. Find the kth element from the last.
```
public static LinkedList getKthLastElement(LinkedList head, int k) {
    if (head == null || k < 1) {
        return null;
    }

    LinkedList current = head;
    LinkedList prev = head;


    for (int i = 0; i < k - 1; i++) {
        current = current.next;
        if (current == null) {
            return null;
        }
    }

    while (current.next != null) {
        prev = prev.next;
        current = current.next;
    }

    return prev;
}

```


Note: Same assumptions as above.

## Test/QA Questions

4. What steps would you take to automate testing?

5. What are the criteria under which you shouldn’t automate a test?

6. You are given a large amount of log files, how would you find the top ten visited links?

7. If you are asked to test google search bar, how would you test it?

8. In your view, what are the pros and cons of automating a test at UI level?

9. What are the software testing tools that you use in your own projects, and why?


