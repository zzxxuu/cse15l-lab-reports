## Lab Report 3

### Streamlining ssh Configuration

![Image](截屏2022-05-08 下午3.04.04.png)

I edited the file by entering the host and hostname. 

![Image](截屏2022-05-16 上午1.15.34.png)

ieng6, as my alia, loged me in my account without using my username and password. 

![Image](截屏2022-05-16 下午6.05.11.png)
![Image](截屏2022-05-16 下午6.05.53.png)
![Image](截屏2022-05-16 下午6.06.21.png)
![Image](截屏2022-05-16 下午6.06.40.png)
![Image](截屏2022-05-16 下午6.07.09.png)
I was able to use scp to move the file to the remote computer using the alia. 


### Setup Github Access from ieng6

![Image](截屏2022-05-08 下午3.11.06.png)

The key was stored in my user account. 


![Image](截屏2022-05-16 下午6.15.27.png)
![Image](截屏2022-05-16 下午6.15.50.png)

The private key is in the remote computer with ssh directry. As I shown here with `ls` command, you can tell becauae it is listed under there. 

![Image](截屏2022-05-16 下午6.08.52.png)
![Image](截屏2022-05-16 下午6.11.05.png)
![Image](截屏2022-05-16 下午6.11.38.png)
![Image](截屏2022-05-16 下午6.12.02.png)
![Image](截屏2022-05-16 下午6.12.38.png)
![Image](截屏2022-05-16 下午6.13.14.png)

Above are showing using the `git` command to commit and push a change while logging into my ieng6 account


![Image](截屏2022-05-08 下午3.16.37.png)
![Image](截屏2022-05-08 下午3.17.16.png)

I used `vim` to change the `testfile`. To perform the follwing operations, `git add test-file.md` and `git commit` were used. 

### Copy Whole directories with scp -r

![Image](截屏2022-05-16 上午1.25.57.png)
![Image](截屏2022-05-16 上午1.26.41.png)
![Image](截屏2022-05-16 上午1.27.11.png)
![Image](截屏2022-05-16 上午1.27.39.png)
![Image](截屏2022-05-16 上午1.28.17.png)
![Image](截屏2022-05-16 上午1.29.04.png)
![Image](截屏2022-05-16 上午1.32.04.png)
![Image](截屏2022-05-16 下午6.13.41.png)

Above are the process of coping `markdown-parser` to the remote computer. You can see that all of the required files are there when I use `ls` command. 

![Image](截屏2022-05-16 上午1.35.25.png)
![Image](截屏2022-05-16 上午1.36.11.png)
![Image](截屏2022-05-16 上午1.36.36.png)

After logging into my `ieng6` account, I was able to compile and run within remote computer. And I used the Linux/Max commands since the terminal computer is that category.

![Image](截屏2022-05-16 上午1.39.19.png)
![Image](截屏2022-05-16 上午1.39.53.png)
![Image](截屏2022-05-16 上午1.40.36.png)
![Image](截屏2022-05-16 上午1.41.00.png)
![Image](截屏2022-05-16 上午1.41.23.png)

So, I used this command to copy the directory and run the test in one line:  `scp -r . ieng6:markdown-parse2; ssh ieng6 "cd markdown-parse2; /software/CSE/oracle-java-17/jdk-17.0.1/bin/javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java; /software/CSE/oracle-java-17/jdk-17.0.1/bin/java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest"`