# commonmark-spec Test Debugging

*click* [here](https://claireconner.github.io/cse15l-lab-reports/) *to go back to index page* 


## How I found the tests
I found the tests by using `diff` on the results of running a bash for loop. To do this, I created a file of the results of running the test files in each version of markdownParse. Then, I used diff to compare these two files. 

## Test 22

![Image](lap-rep5-photo/test1Output.png)
**Actual Output**

From the provided markdown-parse repository, the expected output is []. From my markdown-parse repository the expected output is [/bar\\* "ti\\*tle"]. 

**Expected output**

The expected output, according to commonMark, is [bar\*], so they are both wrong. 

**How To Fix**

*This is my markdown-parse repository in which I will show a bug*

My implementation of markdownParse fails to account for the index of "\\" which is important because it negates whatever character comes after. 
![Image](lap-rep5-photo/test22Bug.png)
It should add code that accounts for the backslash. 


## Test 2


