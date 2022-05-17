------
# Lab Report 3
------
## 
# Streamlining ssh Configuration

1. While not signed into ssh, try entering ``~/.ssh/config`` which will look like: 
>If you change the phrase next to Host, then enter ``ssh + whatever is to the right of Host``

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-08%20124247.png)

2. Next sign in using the next alias you created:

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-08%20122039.png)

3. Then you can use ``scp`` to copy the file containing your alias

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-16%20190330.png)

# Setup Github Access from ieng6
1. Go to GitHub user account and check where your public key is stored:

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-16%20190629.png)

2. Check where it is stored within your own user account on ssh:

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-16%20191503.png)

3. Now check if your git commands work on ssh account:

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-16%20191315.png)

4. Result of Commiting from ssh account should look like this on github:

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-16%20191920.png)


# Copy whole directories with scp -r

1. Enter ``scp -r *.java *.md lib/ alias from part 1+:markdown-parse`` which will copy the entire directory to you ieng6 account

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-08%20155207.png)

2. login to your ssh account and run the tests of your repository tests:

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-16%20194406.png)

3. You can combine the two previous steps into one command using: ``scp -r *.java *.md lib/ alias from part 1+:markdown-parse; + ssh; + enter directory; + java; + and javac commands``

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-16%20194753.png)

> Git Add: 

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/oie_BbE2FM0JcBAO.png)


> Git Push: 

![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-05-16%20195005.png)

-----
