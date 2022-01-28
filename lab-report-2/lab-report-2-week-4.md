# Lab Report 2 - Week 4

# How to utilize debugging to fix a bug 
Yonghyeon Choi / PID : A17010613

## Code Change 1 : File including image link

> Code Change 
![Image](lab-report-2/Bug1Fixed.png)

> Failure-Inducing Input File Link
[Click](https://github.com/choi8616/markdown-parse/blob/main/test-file2.md)

> Failure-Inducing Input Symptom
![Image](lab-report-2/Bug1-ImageLink.png)

> Relationship Description

- First bug was encounterd when `test-file2.md`, including image url, was used as an argument. It printed out the image url even though it wasn't a link. The bug 
  occured because `getLinks` method regarded the image url as a link also, since image url was also in the parentheses after brackets. To fix this bug, we tried to
  find a difference of property between a normal link and a image url. The difference was that image url included a exclamation mark before the brackets. Therefore,
  we added a new `int` value that finds the index of the exclamation mark. Using this `int` value, we determined if the exclamation mark exists or not using a 
  `if-statement`. 
  
  
