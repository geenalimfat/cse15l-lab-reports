# **Lab Report 4**
## **Part 1: Changing the name of the `start` parameter and its uses to `base`**   
In this lab, we change the name of the `start` paramter in the `getFiles` in the file `DocSearchServer.java`. 
**Note: The photos below are after the commands have been run. 

1. The command `vim DocSearchServer.java` was entered into terminal which opened the file `DocSearchServer.java` in vim. In the picture below, we see the file opened in normal mode.
![Image](Images/lab%204/in-vim.png)
2. Next, the command `/start <Enter>` was inputted. This command will search for the word `start` in the file and `<Enter>` would enact the command.
![Image](Images/lab%204/%3Astart.png)
3. The command `dw` was entered next which deleted the word `start`.
![Image](Images/lab%204/first-dw.png)
4. Then, the command `i base <enter>` enters insert mode in vim so we can type in the word `base` to replace the word `start`.
![Image](Images/lab%204/first-i-spacebar-base.png)
5. After inserting the `base`, we press `<esc>` to  exit insert mode and press the key `<n>` which takes us to the next occurence of of the word `start` where we will now repeat the same process as above. 
![Image](Images/lab%204/first-escape-n.png)
6. The command `dw` deletes this occurence of `start`.
![Image](Images/lab%204/second-dw.png)
7. The command `i base <enter>` enters insert mode where we can type in the word `base` to replace `start`. 
![Image](Images/lab%204/second-i-base.png)
8. `<esc> <n>` exits insert mode and takes us to the next occurence of `start`, which happens to be the last occurence.
![Image](Images/lab%204/third%20escape.png)
9. The command `dw` deletes the word `start`.
![Image](Images/lab%204/third-dw.png)
10. `i base <enter>` enters insert mode so we can type the word `base` in. We can see in this photo below that we are in insert mode because of the text that says **INSERT** at the bottom of the page.
![Image](Images/lab%204/third-i-base.png)
11. As the last step to save the changes we made to the file, we enter the command `:wq <enter>` to save the changes we made and exit out of vim. We see in the photo that we are no longer seeing the file `DocSearchServer.java` in terminal and are instead in our regular terminal.
![Image](Images/lab%204/wq.png)

## **Part 2**
1. Which of these two styles would you prefer using if you had to work on a program that you were running remotely, and why?   
I prefer editting the file in Visual Studio Code first and then using `scp` to send over a copy to the remote server. I think it's easier to use Visual Studio Code to edit the file directly rather than using Vim because sometimes I still forget the commands for Vim and it's just easier to move the cursor to the places that I need it to be in. It's also easier since I can edit it directly without having to enter insert mode and the file with save automatically as opposed to Vim where I need to enter different modes and remember to save my changes to the file. 
2. What about the project or task might factor into your decision one way or another? (If nothing would affect your decision, say so and why!)   
If the project started in the remote server and had different files that I had to use in the remote server, then I would use Vim because the files are already in the remote server. Also, since there are other files that are in the remote server which the file I'm editting relies on, then it's easier to test the file I'm editting since all the files are already in the same place. If I had to use `scp` to send all the files over to my local server where I could use Visual Studio Code, it would not only be tedious, but I could possibly forget to send over some files which will cause errors in my tests. 
