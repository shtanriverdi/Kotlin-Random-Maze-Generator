# Kotlin Random Maze Generator
An automated maze generation algorithm method to create random mazes in Kotlin

This is a simple maze generator written in Kotlin with the purpose of learning Kotlin language basics as well as having some grasp and applying of algorithms and data structures knowledge.

This DFS class contains both Iterative and Recursive implementation of the DFS traversal algorithm, so you can read the code and learn both of them, since recursion can cause stack overflow problems, I wanted to write and learn both. 

When you run the code you will see the output of each step of what dfs is doing as following;

```
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██             ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██    ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██    ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██    ██ ██ ██ ██ ██ ██ ██ 
██             ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██             ██ ██ ██ ██ 
██    ██ ██    ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██    ██ ██ ██ ██ ██ ██ ██ 
██             ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██                      ██ 
██    ██ ██    ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██    ██ ██ ██ ██ ██ ██ ██ 
██             ██ ██ ██ ██ ██ ██ ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██                      ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██             ██ ██ ██ ██ ██    ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██                      ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██             ██ ██             ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██                      ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██             ██ ██             ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██                      ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██             ██ ██             ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██ ██ ██ ██             ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██                      ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██             ██ ██             ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██                      ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██                      ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██             ██ ██             ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██                      ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██                      ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██             ██ ██             ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 
██    ██ ██                      ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██             ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██ ██ ██ ██ ██ ██ ██    ██ 
██    ██ ██                      ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██    ██ ██    ██ ██ ██ ██ ██    ██ 
██             ██ ██             ██ 
██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ 

Process finished with exit code 0
```
