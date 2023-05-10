# **Lab Report 3**
## grep -i (ignore case)
This option tells grep to ignore the case of the thing you are searching for.

I found this option by asking chatGPT "what are 4 grep command line options"

```
$ grep -i "nothing" chapter-2.txt
                in the world today and the worst terrorists are the Americans. Nothing could stop
                as entirely material, arguing that Western society possesses "nothing that will
                inspired by Bin Ladin. They were promptly executed. Though nothing proves that Bin
```
In this example, grep was searching for the word "nothing" in the file `chapter-2.txt` and returned a line with the 'n' capitalized and two other lines with 'nothing' in all lower case.

```
$ grep -i "VIOLENT" chapter-2.txt
            It is the story of eccentric and violent ideas sprouting in the fertile ground of
                for peaceful opposition, forcing their critics to choose silence, exile, or violent
                especially clear in Egypt. Confronted with a violent Islamist movement that killed
                vision of their faith, not the violent sectarianism of Bin Ladin. Among Arabs, Bin
                violent Islamist extremists came from all the groups represented in Bin Ladin's
```
In this example, grep was searching for the word "VIOLENT" in the file `chapter-2.txt` and returned lines with the word in all lower case.

Both examples demonstrated that this option is helpful when you wan to find instances of a word appearing in a file but can't remember or don't care about the case of the word.


## grep -r (recursive)
This option tells grep to search all files and directories recursively, similar to the `find` command 

I found this option by asking chatGPT "what are 4 grep command line options"

```
$ grep -r "deterministic"
biomed/1471-2180-3-11.txt:        derivation of a set of deterministic equations that
biomed/1472-6793-2-18.txt:        with deterministic synchronization when compared with
biomed/1472-6793-2-18.txt:          deterministic properties of the RR series on the LF-HF
biomed/1472-6793-2-18.txt:          to the random order of RR intervals, deterministic phase
biomed/1472-6793-2-18.txt:          short, and consequently testing for deterministic phase
biomed/gb-2001-2-4-research0010.txt:          termination). As the model is deterministic, it is not
biomed/gb-2002-3-11-research0059.txt:            deterministic clustering results, in contrast to the
biomed/gb-2002-3-12-research0087.txt:          identified by MEME. Gibbs sampling is non-deterministic
biomed/gb-2002-3-9-research0048.txt:        deterministic; and third, the quantile-based approach of
government/Env_Prot_Agen/tech_sectiong.txt:deterministic linear programming model of the U.S. electric power
plos/journal.pbio.0020164.txt:        deterministic analyses.
plos/journal.pbio.0020206.txt:        biases are deterministic, there are plenty of ‘successful’ gene family clusters that
```
In this example, grep is searching through all of the files and directories in `.\technical` for the word "deterministic" and returns the line containing the word as well as the relative path to the file it is in.

```
$ grep -r "FOREWORD"
government/About_LSC/Comments_on_semiannual.txt:FOREWORD
government/Gen_Account_Office/Statements_Feb28-1997_volume.txt:FOREWORD
```
In this example, grep is searhing through all of the files and directories in `.\technical` for the word "FOREWORD" and returns the lines cointaining the word as well as the relative path to the file it is in.

Both examples demonstrate that this option is helful when you want to find the files a specific word appears in and the line it is in.


## grep -n (line number)
This option tells grep to print the line numbers of the matched lines.

I found this option by asking chatGPT "what are 4 grep command line options"

```
$ grep -n "COUNTERTERRORISM" chapter-3.txt
4:            COUNTERTERRORISM EVOLVES
162:                in the 1970s. Two years after Hoover's death in 1972, congresCOUNTERTERRORISM 
252:                desCOUNTERTERRORISM
435:            Midlevel INS employees proposed comprehensive counterterrorism proCOUNTERTERRORISM
1033:                opposed Shultz, who made little headCOUNTERTERRORISM
```
In this example, grep is searching for the word "COUNTERTERRORISM" in the file `chaper-3.txt` and returns the line and line number it appears in.

```
$ grep -n "Volunteers" A_Perk_of_Age.txt
12:caregivers as well. Volunteers offer advice on legal questions,
```
In this example, grep searches for the word "Volunteers" in the file `A_Perk_of_Age.txt` and returns the line and line number it appears in.

Both examples demonstrate that this is helpful when you want to find the line number a word appears on so that you can navigate to it in the actual file.


## grep -w (word match)
This option tells grep to match only whole words.

I found this option by asking chatGPT "what are 4 grep command line options"

```
$ grep -w "COUNTERTERRORISM" chapter-3.txt
            COUNTERTERRORISM EVOLVES
```
In one of the previous examples when "COUNTERTERRORISM" was used as the argument for grep -n, it returned 5 lines the word occured in. However, unlike the previous example which returned lines that contained words like "desCOUNTERTERRORISM" and "congresCOUNTERTERRORISM", this example only returned the line in which "COUNTERTERRORISM" appeared as its own word, not attached to anything else.

```
$ grep -w "respect" journal.pbio.0020001.txt
        examined it in respect to worldwide publications. In this case, the United States
```
In this example, grep searched for the word respect in the file `jornal.pbio.txt` and returnd the line it appeared in. In this file, the word "respectively" which contains the word "respect" also appeared in the file, yet it wasn't printed to the terminal because it wasn't just the word "respect" on its own.

Both examples demonstrate that this option is useful when the word you want to find is a single letter or common root for other words but you just want to find the letter or root word itself.
