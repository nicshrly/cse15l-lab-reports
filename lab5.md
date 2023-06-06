# **Lab Report 5**
## Original Student Post
What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?

  Predator PH315-54, Windows 10, Chrome, VScode, bash terminal

Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead.
Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.

  I am trying to isolate the second line of the JUnit output that has the E's and dots so that I can count the amount of
  errors the student has and give them a grade. The JUnit output is in a file called output.txt and I tried using the head 
  and tail commands to extract the line I want and redirect it to rsult.txt. However, when I run the commands, result.txt 
  comes back empty. I made sure to put the right numbers when using the head and tail commands because i counted them. Im 
  not sure why there is no output.
  
  ![Image](lr5_1.png)
  
  ![Image](lr5_2.png)

Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line 
arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.

  Terminal command: 
  
  $ bash grade.sh https://github.com/ucsd-cse15l-f22/list-methods-lab3
  
  Shell file commands:

  head -n 2 output.txt > result.txt
  
  tail -n 1 result.txt > result.txt
  
 ## Leading TA Response
 Is the error caused by both the head and tail commands, or could it be just one that is causing the error? Try adding a cat command in between
 the head and tail commands to see how each modies the result.txt file.
 
 ## Student Follow-up Response
 I added the cat command and it seems like the head command is working as intended since it outputs the first two lines of the JUnit output. The
 error must be occuring when I use the tail command and redirect the input back into the result.txt file.
 
 ![Image](lr5_3.png)
 
 ## TA Solution
 Try redirecting the output of the tail command into a different file other than result.txt.
 
 ## Studnet Follow-up Response
 Error fixed, ty! :3 
 
 ![Image](lr5_4.png)
 
 ![Image](lr5_5.png)
 
 ## Setup Info
 I used a fork of the list_examples_grader directory from lab 6. The relevant code from the grade.sh file I used is as follows:
 
 
