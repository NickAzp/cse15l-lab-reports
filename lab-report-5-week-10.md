# Test 1

### How I found the test with different results

I found this test through manually searching and finding a test that I think my code did not account for. In this case, it was not accounting for slashes in the link.

### Link to the test-file with different results

https://github.com/nidhidhamnani/markdown-parser/edit/main/test-files/509.md

### Expected output

![Image1](file1.png)

Should be [title]

### My implementation output

![Image2](file2.png)

### Implementation for week 9 output

![Image6](file6.png)

### Correctness of implementation

Both implementations are incorrect.

### If implementation(s) have bug. Description of bug in 2-3 sentences with screenshot of where code needs to be fixed.

The bug is from my implementation not accounting for slashes in the link. This could be fixed with adding a loop to remove the slashes after the links have been found. This would ensure my code still functions as it would only impact what's inside the link.

![Image8](file8.png)

# Test 2

### How I found the test with different results

I found this test through manually searching and finding a test that I think my code did not account for. In this case, it was the extra brackets in the file that I think may have caused an error.

### Link to the test-file with different results

https://github.com/nidhidhamnani/markdown-parser/edit/main/test-files/531.md

### Expected output

![Image3](file3.png)

Should be [/url, /url]

### My implementation output

![Image4](file4.png)

### Implementation for week 9 output

![Image5](file5.png)

### Correctness of implementation

Both implementations are incorrect.

### If implementation(s) have bug. Description of bug in 2-3 sentences with screenshot of where code needs to be fixed.

The problem with my code is that I rely off of the indexing of brackets and parathesis to determine the links. This causes an error when there's extra brackets like in this test file. A for loop, at the start before the indexing of the brackets is used, to get rid of the extra brackets may solve this issue.

![Image7](file7.png)
