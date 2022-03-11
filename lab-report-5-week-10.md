# **LAB 5 REPORT**


We are going to be comparing the results of two `MarkdownParse.java` implementations when they run the tests from the `test-files` folder.

#### **STUDENT REPOSITORY:** [https://github.com/m1ma0314/markdown-parse](https://github.com/m1ma0314/markdown-parse)

<br/>

We found the differences between the test results by using the program `diff`, which compares two files line by line and produces an output that shows exactly where the outputs vary.

This is what we entered on the terminal or Command Prompt if `results.txt` is the output of `test-files`:
```
diff some-markdown-parse/results.txt other-markdown-parse/results.txt > resultsDiffs.txt
```
<br/>

### **Test File #490**
```
[link](<foo
bar>)
```
#### **student results:** 
![image](Screenshot2022-03-10144940.png)

#### **class results:** 
![image](Screenshot2022-03-10145629.png)

#### **EXPECTED OUTPUT** 
![image](Screenshot2022-03-10160011.png)

Using CommonMark, we see that the class implementation is correct because it produces `[]`, as `<foo
bar>` is not going to be recognized as a link. 

The *bug* in the student implementation 

<br/>

### **Test File #510**
```
[link] (/uri)
```

#### **student results:** 
![image](Screenshot2022-03-10160354.png)

#### **class results:** 
![image](Screenshot2022-03-10160617.png)

#### **EXPECTED OUTPUT** 
![image](Screenshot2022-03-10160512.png)

<br/>

### This marks the end of CSE 15L! 🎉

Describe which implementation is correct, or if you think neither is correct, by showing both actual outputs and indicating what the expected output is.

For the implementation that’s not correct (or choose one if both are incorrect), describe the _bug (the problem in the code). You don’t have to provide a fix, but you should be specific about what is wrong with the program, and show the code that should be fixed.
