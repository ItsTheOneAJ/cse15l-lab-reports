------
# Markdown Switch With Group 5
------
> ### Our Groups [Markdown](https://github.com/aaronchan32/markdown-parser)

> ### Group 5's [Markdown](https://github.com/httrieu/markdown-parser)
### Test Cases for Snippet 1, 2, and 3: 
![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-22%20140127.png)

## Snippet 1
#### Our group:

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-22%20140814.png)
Expected: `[url.com, 'google.com, google.com]`

Output: `['google.com, google.com, ucsd.edu]`

> *Failure!!!*

#### Group 5:
![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-22%20141917.png)
Expected: `[url.com, 'google.com, google.com, ucsd.edu]`

Output: `['google.com, google.com, ucsd.edu]`

> *Failure!!!*

## Snippet 2
#### Our group:

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-22%20142504.png)
Expected: `[a.com, a.com(()), example.com]`

Output: `[a.com, a.com((, example.com]`

> *Failure!!!*

#### Group 5:
![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-22%20143010.png)
Expected: `[a.com, a.com(()), example.com]`

Output: `[a.com, a.com((, example.com]`

> *Failure!!!*

## Snippet 3
#### Our group:

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-22%20150009.png)
Expected: `[]`

Output: `[https://ucsd-cse15l-w22.github.io/]`

> *Failure!!!*

#### Group 5:
![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-22%20150431.png)
Expected: `[https://twiter.com, https://ucsd-cse15l-w22.github.io/]`

Output: `[https://ucsd-cse15l-w22.github.io]`

> *Failure!!!*

## Q&A:

* Snippet 1: 

Q: Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.
>A: **I believe that only a small portion of code is needed to fix this problem. If the end bracket comes before the start braket, then it should be a valid link.**

* Snippet 2: 

Q: Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.
>A: **This is a small change, if you are able to pop the extra brackets and parenthesis within the code. By checking if it has a closed bracket after a open, if there is another open then it will pop that if it is between an open and the closed bracket or parenthesis.**

* Snippet 3: 

Q: Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.
>A: **A small change will help, it can check if there is a new line within the file, and if so trim the string it adds to the array.**






------
