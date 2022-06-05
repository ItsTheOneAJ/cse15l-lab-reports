----
# Lab Report 5
----

### To find differences between the program outputs you can use the vim command:
> ### `diff (file 1 name)/results.txt (file 2 name)/results.txt`

### **Test File with different Output:**
> ### **[File for Test 194](https://raw.githubusercontent.com/nidhidhamnani/markdown-parser/main/test-files/194.md)**
> ### **[File for Test 194](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/489.md)**


## Test Difference 1:

The first difference is on `194.md`.

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-06-05%20110257.png)

According to CommonMark the correct output was produced by my implementation because the expected output was: `[]` , but the provided MarkdownParse's output was `[url]`.

#### The Bug and Possible Fix Area:

> The problem with the provided MarkdownParser's method is: when a second closed bracket appears prior to the link for the webpage appears it does not close off. It continues until it finds the parenthesis, which adds unneccessary parks into the link base. 

If you add a check to see if a closed parenthesis comes after a open and closed brakcet, only then do you add it to the list.
![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-06-05%20112160.png) 


## Test Difference 2:

The second difference is on `489.md`.

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-06-05%20113355.png)
*The Left output is mine, the right is the provided*

According to CommonMark the correct output was produced by the provided MarkDownParser's implementation because the expected output was: [], but my output was [foo \n bar].

#### The Bug and Possible Fix Area:

> The problem with my MarkdownParser's method is: when a new line is within the text it still catches the link as a valid input. When in fact it should not catch it at all, it should break if there is a new link between the parenthesis.

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-06-05%20114032.png) 

------
