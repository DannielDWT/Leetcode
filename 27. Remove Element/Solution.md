﻿# Solution

```java
class Solution {
    public int removeElement(int[] nums, int val) {
        int length = 0;
        for (int i = 0; i < nums.length; ++i)
        {
            if (nums[i] == val)
                continue;
            nums[length++] = nums[i];
        }
        return length;
    }
}
```

It is neccessary to read the code in leetcode Solution

```java
public int removeElement(int[] nums, int val) {
    int i = 0;
    int n = nums.length;
    while (i < n) {
        if (nums[i] == val) {
            nums[i] = nums[n - 1];
            // reduce array size by one
            n--;
        } else {
            i++;
        }
    }
    return n;
}
```

the diffecrence will be explained in README.md




