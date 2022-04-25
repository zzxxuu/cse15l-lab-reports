## Lab Report 2


### First Code Change
![Image](截屏2022-04-24 下午4.49.45.png)

* Link to failing test file: [https://github.com/zzxxuu/markdown-parser/blob/main/test-file4.md]https://github.com/zzxxuu/markdown-parser/blob/main/test-file4.md


![Image](截屏2022-04-24 下午4.55.05.png)
* The problem here is that it is supposed to return more than just the URL links. However, the bug here only returned the links as I showed above. 




### Second Code Change
![Image](截屏2022-04-24 下午3.33.47.png)

* Link to the failing test file: [https://github.com/zzxxuu/markdown-parser/blob/main/test-file2.md]https://github.com/zzxxuu/markdown-parser/blob/main/test-file2.md


![Image](截屏2022-04-24 下午4.32.35.png)
* The problem here is that the code never reaches the end of the infinite while loop, causing the error of heap space. Therefore, our group made this if statement to break the loop if it reaches the end of it. 


### Third Code Change
![Image](截屏2022-04-24 下午3.34.57.png)

* Link to the failing test file: [https://github.com/zzxxuu/markdown-parser/blob/main/test-file3.md]https://github.com/zzxxuu/markdown-parser/blob/main/test-file3.md


![Image](截屏2022-04-24 下午4.38.24.png)
* The bug here is that the index is out of bounds. There should no be -1 index in our file. 