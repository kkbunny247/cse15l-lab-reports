# **LAB 4 REPORT**


### **The Setup**

We are going to be running more tests against our `MarkdownParse.java` file as well as another student's `MarkdownParse.java` file.
#### **my repository:** [https://github.com/kkbunny247/markdown-parse](https://github.com/kkbunny247/markdown-parse)

#### **reviewing repository:** [https://github.com/sallada1/markdown-parse](https://code.visualstudio.com/)

<br/>

From the following 3 Markdown files, the code should pull the links.

#### **Test 1** 
```
`[a link`](url.com)

[another link](`google.com)`

[`cod[e`](google.com)

[`code]`](ucsd.edu)
```
#### **Test 2** 
```
[a [nested link](a.com)](b.com)

[a nested parenthesized url](a.com(()))

[some escaped \[ brackets \]](example.com)
```

#### **Test 3** 
```
[this title text is really long and takes up more than 
one line

and has some line breaks](
    https://www.twitter.com
)

[this title text is really long and takes up more than 
one line](
    https://ucsd-cse15l-w22.github.io/
)


[this link doesn't have a closing parenthesis](github.com

And there's still some more text after that.

[this link doesn't have a closing parenthesis for a while](https://cse.ucsd.edu/



)

And then there's more text
```
<br/>

### **Determining Our Tests**

From the CommonMark demo site ([https://spec.commonmark.org/dingus/](https://spec.commonmark.org/dingus/)), we can figure our what to put in the JUnit's test in our `MarkdownParseTest.java` file.

![image](Screenshot2022-02-23172911.png)