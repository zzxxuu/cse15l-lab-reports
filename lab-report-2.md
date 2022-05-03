## Lab Report 2


### First Code Change
![Image](截屏2022-04-24 下午4.49.45.png)

* Link to failing test file: [https://github.com/zzxxuu/markdown-parser/blob/main/test-file4.md](https://github.com/zzxxuu/markdown-parser/blob/main/test-file4.md)


![Image](截屏2022-05-02 下午4.52.57.png)
* The problem here is that it is supposed to return just the URL links, but it is returning both the image and URL links.  The bug is that the code does not differentiate between image and URL links. What me and my partner did here is allow the code to identify "!" to differentiate between image and URL and only return URL.
The failure-inducing file containd both of these, which is why we have the output shown above.  




### Second Code Change
![Image](截屏2022-04-24 下午3.33.47.png)

* Link to the failing test file: [https://github.com/zzxxuu/markdown-parser/blob/main/test-file2.md](https://github.com/zzxxuu/markdown-parser/blob/main/test-file2.md)


![Image](截屏2022-05-02 下午4.39.59.png)
* The problem here is that the code never reaches the end of the infinite while loop, causing the error of heap space. Therefore, all of the elements in the test file would be go over and the code will never stop. Therefore, our group made this if statement to break the loop if it reaches the end of it. 


### Third Code Change
![Image](截屏2022-04-24 下午3.34.57.png)

* Link to the failing test file: [https://github.com/zzxxuu/markdown-parser/blob/main/test-file3.md](https://github.com/zzxxuu/markdown-parser/blob/main/test-file3.md)


![Image](截屏2022-05-02 下午4.42.38.png)
*  The correction of the code is for when the test files contain parentheses but no link. This was the case for test file 3, it only has couple sentences and []. The code failed initially for it skips this situation where [] being used incorrectly, which results in indexoutbounds for the code would not stop even if the input does not contain the required parenthese. 