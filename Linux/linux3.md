### **SEEING THE WORLD AS SHELL SEES**  
Lets look at some of the magic that occurs in the command line when we press ENTER key.
### **Expansion**  
- Each time we type a command & press Enter key, bash performs several substititutions upon text before command is executed. The process that makes it happen is called expansion
- To demonstrate this lets try
```
echo Welcome to Linux by gopi  
```
![](./images/img10.png)  

- Note: Images with terminal in black (git bash) is connected to ubuntu 18 and Images with terminal in blue (powershell) is connected to centos 8.1  
- Now lets execute the following  

![](./images/img11.png)  

What happened? * is a wild card character, so your bash will try to find/match any characters in the files present in current working directory (cwd).  

So initially when we executed there were no files in cwd, so it printed *. Then we created two files and execute echo * again, now * will match any file name in cwd so it printed the file names  


Pathname Expansion: The mechanism by which wild cards work is called as pathname expansion
Lets experiment with the following
```
create two directories Videos and Documents in the cwd  
```

