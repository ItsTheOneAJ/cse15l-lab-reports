------
# Lab Report 2
------
## 
# Initial Error Found
## New change:

![image](https://github.com/ItsTheOneAJ/markdown-parser/blob/main/Screenshot%202022-04-24%20222504.png)

1. [Link](https://github.com/ItsTheOneAJ/markdown-parser/blob/main/testTwo-copy.md) to the failure-induced input
2. Screenshot for symptoms: 
![image](https://github.com/ItsTheOneAJ/markdown-parser/blob/main/Screenshot%202022-04-24%20220637.png)
4. The scanner only searched to see if the end parenthesis wasnt there that it would break, but not if there was no open parenthesis. This created an infinite loop of searching the file until it overloaded the system. 

# Second Error found
## New Change: 

![image](https://github.com/ItsTheOneAJ/markdown-parser/blob/main/Screenshot%202022-04-24%20222044.png)
1. [Link](https://github.com/ItsTheOneAJ/markdown-parser/blob/main/testTwo-copy.md) to the failure-induced input
2. Screenshot for symptoms: 
![image](https://github.com/ItsTheOneAJ/markdown-parser/blob/main/Screenshot%202022-04-24%20220637.png)
5. This change only checked if the brackets were both there, creating in ifinite loop to look for both the end/open parenthesis within the file. Overloading the file and creating a system break. 

# Third Error
## New Change: 

![image](https://github.com/ItsTheOneAJ/markdown-parser/blob/main/Screenshot%202022-04-24%20215649.png)
1. [Link](https://github.com/ItsTheOneAJ/markdown-parser/blob/main/testTwo.md) to the failure-induced input
2. Screenshot for symptoms: 
![image](https://github.com/ItsTheOneAJ/markdown-parser/blob/main/Screenshot%202022-04-24%20225443.png)
4. The system could not recognize that there was a parenthesis and bracket within the link area, creating an improper break. It should have checked whether or not there was a close bracket after it and before a new open bracket to make sure that the link was correctly created.  


-----
