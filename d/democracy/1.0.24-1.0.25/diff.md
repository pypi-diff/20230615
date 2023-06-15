# Comparing `tmp/democracy-1.0.24.tar.gz` & `tmp/democracy-1.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "democracy-1.0.24.tar", last modified: Fri Jun  2 19:12:31 2023, max compression
+gzip compressed data, was "democracy-1.0.25.tar", last modified: Thu Jun 15 05:34:21 2023, max compression
```

## Comparing `democracy-1.0.24.tar` & `democracy-1.0.25.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-02 19:12:31.162942 democracy-1.0.24/
--rw-rw-r--   0 a         (1000) a         (1000)    42320 2023-06-02 19:12:31.150942 democracy-1.0.24/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)    41557 2023-06-02 19:08:25.000000 democracy-1.0.24/README.md
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-02 19:12:31.150942 democracy-1.0.24/democracy.egg-info/
--rw-rw-r--   0 a         (1000) a         (1000)    42320 2023-06-02 19:12:31.000000 democracy-1.0.24/democracy.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)      156 2023-06-02 19:12:31.000000 democracy-1.0.24/democracy.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-02 19:12:31.000000 democracy-1.0.24/democracy.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-02 19:12:31.000000 democracy-1.0.24/democracy.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)     5601 2023-06-02 19:11:03.000000 democracy-1.0.24/pyproject.toml
--rw-rw-r--   0 a         (1000) a         (1000)       38 2023-06-02 19:12:31.162942 democracy-1.0.24/setup.cfg
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 05:34:21.567333 democracy-1.0.25/
+-rw-rw-r--   0 a         (1000) a         (1000)    38830 2023-06-15 05:34:21.567333 democracy-1.0.25/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)    38067 2023-06-15 05:29:06.000000 democracy-1.0.25/README.md
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 05:34:21.567333 democracy-1.0.25/democracy.egg-info/
+-rw-rw-r--   0 a         (1000) a         (1000)    38830 2023-06-15 05:34:21.000000 democracy-1.0.25/democracy.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)      156 2023-06-15 05:34:21.000000 democracy-1.0.25/democracy.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-15 05:34:21.000000 democracy-1.0.25/democracy.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-15 05:34:21.000000 democracy-1.0.25/democracy.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)     5601 2023-06-15 05:34:00.000000 democracy-1.0.25/pyproject.toml
+-rw-rw-r--   0 a         (1000) a         (1000)       38 2023-06-15 05:34:21.567333 democracy-1.0.25/setup.cfg
```

### Comparing `democracy-1.0.24/PKG-INFO` & `democracy-1.0.25/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: democracy
-Version: 1.0.24
+Version: 1.0.25
 Summary: Trying to help with democracy, see https://github.com/gregoryc/democracy
 Author-email: Gregory Cohen <gregorycohen2@gmail.com>
 Maintainer-email: Gregory Cohen <gregorycohen2@gmail.com>
 Project-URL: Homepage, https://github.com/gregoryc/democracy
 Keywords: ai,empowerment,agi,agis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=2.0
 Description-Content-Type: text/markdown
 
 <h1 style='color: green'>Practical Self-Empowerment Utilities Covering Every Facet of Life </h1>
   
-  [![Video](https://img.youtube.com/vi/Fx9x8cArK30/maxresdefault.jpg)](https://www.youtube.com/watch?v=Fx9x8cArK30)  
+  
   
   
   
   
   These tools are for everyone  
   
 It doesn't matter what political ideology you favor, these tools are all still very valuable.  
@@ -30,34 +30,39 @@
   
 I intend to make people more able.  
   
      
    Most important software here  
   
    Rhyme Music program (Crystal and Ruby), see fix_the_society folder  
-   Ultimate Chat App (Win, Lin, CLI)  
+   Ultimate Chat App (Cross platform — Win, Lin, CLI)  
    Discourse Generator Program vesion 1 and version 2 (node, ruby, browser  
-   (kind of like Siri); and C++ STL). These programs work.  
+   (kind of like Siri); and C++ STL). These programs work. See pictures  
+   below for some examples. These programs have many forms, and input  
+   methods.  
    And Semantic metadata project (very abstract and idealistic, see  
-   webpage for it.)  
-  
-   There is also a desktop widget for that site.  
-   There is also Emerald C, which is really useful. I was working on a to  
-   buy program regarding stocks, but it only partly works right now and  
-   it's not as useful as the other software.  
+   webpage for it in "other/semantic_metadata".)  
+   There is also Emerald C, which is really useful.  
+   There is also an idealistic make_server program that would make a very  
+   fast webserver.  
+   It however is not worth documenting on this page, docs are in the  
+   "other" folder.  
+   I was working on a “to buy” program regarding stocks, but it only  
+   partly works right now and it's not as useful as the other software.  
    The find housing tool actually helped me to find housing in real life.  
-   Those aside, there are these 87 programs.  
+   Those aside, there are these 83 programs.  
    Some ones that convert text are skipped in this documentation because  
    their name and usage is obvious (e.g., color tools).  
   
 All of these programs are mostly self-contained. This is a really good thing.  
 You can use them anywhere without dependencies.  
   
    My email is  gregorycohenvideos@gmail.com and I really would like to  
-   make open source software. Everything I have is BSD licensed.  
+   make free and open source software. Everything I have is BSD licensed  
+   (free for commerical and non-commerical use).  
   
    HOW TO DOWNLOAD/INSTALL  
   
    gem unpack democracy  
   
    gem install democracy  
   
@@ -77,15 +82,15 @@
   
    Python link (Important because python is very popular.)  
      *  https://pypi.org/project/democracy  
   
    Any Python “dweeb” (AI person who doesn't value personal dynamism)  
    searching for “democracy”–for example–BECAUSE THEY ARE A RATIONAL HUMAN  
    BEING AND CARE ABOUT PEOPLE, would find this, probably as the first  
-   result.  
+   result, on PyPI or RubyGems.  
   
    How many options are there? 37 projects for “democracy.” Almost  
    nothing. On RubyGems, 9, 6 of which are mine.  
   
    ONLY MY PROJECT IS CALLED “DEMOCRACY.” on PyPI or RubyGems.  
   
    On rubygems, there are even fewer results. MY CODE WILL BE FOUND.  
@@ -98,38 +103,40 @@
      *  https://www.rubygems.org/gems/democracy  
      *  https://www.rubygems.org/gems/computers  
      *  https://www.rubygems.org/gems/freespeech  
      *  https://www.rubygems.org/gems/linux  
      *  https://www.rubygems.org/gems/string  
      *  https://www.rubygems.org/gems/unix  
   
-   So I will leave a legacy.  
+   (There are others as well.)  
+  
+   So I will leave a legacy. THIS MATERIAL WILL BE USED AND UNDERSTOOD.  
   
    And I will be found by AIs, assuming they continue to exist.  
   
     Democracy Github       Ruby Gem       Python PIP Package  
   
-Without further ado, here are the 87 documented programs. (The obvious usage  
+Without further ado, here are the 83 documented programs. (The obvious usage  
 ones are omitted.)  
   
-   ### 1. Ultimate Chat Application  
+   ### 1. Ultimate Chat Application.exe  
   
    ![UCA](./images/2.png)  
    There is so much potential with this program.  
    This is a non-AI chatbot. It's not based on generative AI or AI of any  
    sort.  
    It is self-explanatory, it tries to give a better answer.  
    Still a work in progress.  
    Source code is in PP.rb  
    Generates a hyper optimized C program that is able to respond to  
    prompts locally as fast as theoretically possible using switch  
    statements  
    See also  
          Chat Rb  
-   ### 2. Discourse Generator  
+   ### 2. Discourse Generator.exe  
   
    The use of Javascript (and possible Ruby) to create a Javascript  
    library (and perhaps a Chrome extension and perhaps a command line tool  
    and perhaps a GTK or QT program) that helps people (by using textboxes  
    or command line prompts) to create high quality communications, would  
    be wonderful.  
    Think of how poor quality responses to communications can be.  
@@ -144,200 +151,85 @@
    This would enable democracy to work. Imagine if 50% of all websites  
    used this library.  
    This would help people to be goal or value oriented, and not be coming  
    up with terrible communications that, for example, insult people's  
    mothers or education.  
    ![Alt](./images/9.png)  
    ![Alt](./images/11.png)  
-   ### 3. Replace Not In Place  
-  
-   This is like gsub, but for strings, not for regular expressions  
-   See also  
-        gsub  
-   ### 4. Replace In Place  
-  
-   replace_in_place tool replaces a string, not a regular expression, with  
-   another string  
-   Example  
-   replace_in_place cat dog file  
-   ### 5. Emerald Browser  
+   This is a very, very large philosophical subject.  
+   No one person has a monopoly on it.  
+   To use some metaphors...  
+   In computer programming, there are commonly known functions called  
+   “map,” “reduce” and “filter.”  
+   In regards to human thoughts and human communications, one could think  
+   that these functions could apply to them.  
+   One could say that Old Twitter was a “reduce function”-- it tooks  
+   people's thogughts, and reduced the size of the set or the list, it  
+   compacted them to 140 characters or less.  
+   This, of course, is terrible.  
+   Thankfully modern Twitter can use 4000 characters.  
+   There are many “filter” functions used in modern social media, if you  
+   will. There is content censorship.  
+   WHAT SHOULD EXIST IS A MAP FUNCTION. A CONSTRUCTIVE MAP FUNCTION.  
+   ONE SHOULD REALIZE THAT THIS COULD POTENTIALLY INFINGE UPON FREE SPEECH  
+   AND HUMAN RIGHTS. ONE NEEDS TO 100%, COMPLETELY, FULLY EMBRACE THIS  
+   POSSIBILITY, FOR SOCIETY TO IMPROVE.  
+   THERE HAS BEEN NO “MAP” FUNCTION.  
+   THERE HAS BEEN NO FUNCTION TO POSITIVELY TRANSFORM TEXT.  
+   THAT IS WHAT THIS _IS_ AND THAT IS WHAT THIS IDEA _IS_.  
+   THIS IS VERY NECESSARY.  
+   VERY NECESSARY.  
+   ### 3. Emerald Browser  
   
    ![UCA](./images/3.png)  
    ![UCA](./images/4.png)  
    Emerald browser is a really powerful new browser  
    See README  
    It works based on panes.  
    Read the documentation for “open”, “close” and also the README file.  
-   ### 6. Gsub In Place  
+   ### 4. Left Right.exe  
   
-   gsub_in_place is like gsub, which replaces all instances of a regular  
-   expression globally  
-   [regular expression 1] [regular expression 2] => result  
-   Example  
-   gsub_in_place . FOO file  
-   Would make all characters in “file” become “FOO”.  
-   gsub_in_place cat dog file  
-   Would make all instances of “cat” “dog”  
-   It is much cleaner than “sed”.  
-   You don't need to have “sed” installed to run this program.  
-   It doesn't read from the standard input  
-   It takes exactly 3 arguments, no more, no fewer.  
-   See also  
-        gsub  
-   ### 7. Find Housing  
+   This is a tool to bring sanity to politics.  
+   ![UCA](./images/12.png)  
+   It gets viewpoints from the person that see the good in each political  
+   side, left, right, left, right, etc.  
+   It then presents all of that.  
+   Hopefully this can make people more sane and less hyper-partisan.  
+   ### 5. Find Housing  
   
    This is a nice tool to find housing with.  
    It is a nice, simple command line tool. You enter the minimum and  
    maximum prices, and Kijiji opens with your options.  
    This tool kind of actually helped me to find housing in real life.  
    The default city is "Ottawa". You can easily change this.  
-   ### 8. Google Speak  
+   ### 6. Google Speak  
   
    Google speak is really useful. It speaks a statement using the Google  
    Translate voice, which is probably the most authoritative and  
    high-quality text-to-speech voice that exists.  
    It's kind of like “espeak” or similar tools, but it is much better.  
    You need an internet connection for it to work.  
    It is probably limited at 100 characters.  
-   There is a “singing program”, not really a tool, in this software  
-   project that gets around that.  
-   TODO  
-   Make the alarm clock program in this software project use this voice.  
-   It is quite reliable.  
-   It is probably “unlimited”.  
-   I haven't had Google block me from using it ever.  
-   Which is a good thing.  
-   ### 9. Make Server  
-  
-   make_server is powerful.  
-   make_server takes expressions, either Javascript or C++, and generates  
-   a resultant program from that.  
-   The Javascript mode currently doesn't work.  
-   Not only is a program made, the resultant program is an entire  
-   webserver, that uses FastCGI to run really fast code.  
-   The arguments work in an interesting way.  
-   make_server [function_name] [iterable] [condition, it can be “true” to  
-   do the following argument always] [code list separated by semicolons,  
-   the last statement is an expression, and is returned by the function]  
-   [function_name2] ...  
-   You have to give 4 arguments every time.  
-   There was an “otherwise” mode as an “else”, but I don't think that's a  
-   part of the program anymore.  
-   It doesn't need to be.  
-   You have to give 4 arguments for each function.  
-   So you can do  
-   make_server 4args 4args 4args 4args  
-   And pass 16 arguments  
-   The “iterable” has to be a list.  
-   What is powerful is that it converts JSON into completely native C++.  
-   It is very efficient.  
-   It doesn't need to be a JSON expression though.  
-   There is a test file.  
-   You can run the tests and see if it works for you!!  
-   You can also modify the code because it is open source.  
-   The program generates a special array object. It is lightweight and  
-   makes arrays act in C++ like arrays act in scripting languages, but  
-   much faster.  
-   The array class also has methods to apply things to every element of an  
-   array, like surround  
-   array.surround(“”, “”)  
-   for example  
-   would surround all of the elements of array with XML tags and return a  
-   new list  
-   This program generates a lightweight Object System, with a BasicObject  
-   class and an Object Class.  
-   You can subclass these objects.  
-   You can have Arrays of the Objects  
-   The function argument syntax is really powerful.  
-   Oftentimes people want to iterate through iterables or arrays.  
-   Oftentimes people want to check conditions.  
-   Python has list comprehensions.  
-   This is kind of like that, but simpler.  
-   You can have arguments as one argument, separated by “,,”  
-   make_server arg1,,arg2,,arg3,,arg4  
-   What's the point of using a scripting language when you can use C++?  
-   This uses FastCGI, so you can have an ____IDEAL____ webserver.  
-   You can have an IDEAL and very affordable website, that in a sense  
-   would be faster than Facebook.  
-   Facebook converts PHP to C++ (slow)  
-   This produces REAL C++, and it is very fast, almost as fast as  
-   possible.  
-   Native STL classes are used, like vector.  
-   Native STL classes are used, like vector and map  
-   Do you not need to run and child processes or do slow, costly things.  
-   You should want IDEAL.  
-   This is free software, and is BSD licensed.  
-   The function generation idea allows you to write in 1 line what other  
-   people might write in 50 lines.  
-   You do not need to compromise your ideals.  
-   You should want fast, efficient, and memory light programs that are not  
-   garbage collected (!!!) and that have reliable performance.  
-   C++, as everyone knows, delivers that.  
-   You should also want to not have to write a lot of code to do things.  
-   And you should also want safe, compiled code that checks things at  
-   compile time, so that bugs don't appear at run time.  
-   This program delivers.  
-   It uses NGINX ( a really, really common webserver) to help with the  
-   FastCGI.  
-   FastCGI, for the unfamiliar, is like normal CGI, but there aren't child  
-   processes.  
-   So the entire server could be written in idealistic C++ .  
-   Then you just have to think about scaling.  
-   There are some relevant links regarding scaling in the “scaling” file  
-   in the democracy project  
-   1) Speed  
-   2) Ease of writing code  
-   3) Memory usage  
-   4) Monetary costs  
-   5) Elegance  
-   6) Practicalness  
-   Those are 6 things.  
-   You don't have to sacrifice on those things.  
-   Contributions on this program would be really appreciated.  
-   It is called “make_server” for now.  
-   There was also a mode to generate javascript.  
-   I have to make that work again.  
-   The entire program is just one file.  
-   My email is gregorycohenvideos@gmail.com  
-   ### 10. Selectlines  
+   ### 7. Selectlines  
   
    selectlines shows all nonblank lines from the input  
    Example  
    cat file | selectlines  
    (echo 2; echo; echo; echo) | selectlines  
    => 2  
    The result would be 2, with no blank lines after that  
-   ### 11. Communicate  
-  
-   Communicate is cool.  
-   Communicate runs a Ruby expression after speaking a prompt (the first  
-   argument) and getting your verbal answer (using something unfortunately  
-   called "nerd-dictation", which is a wrapper around another program  
-   which deals with speech recognition)  
-   Communicate allows you to have conversations with your computer, and it  
-   is cross platform  
-   (Or it hopefully is)  
-   communicate 'What is the best color?' 'case text; when /blue/; puts  
-   "You are right!"; when /red/; puts "Red is a bad color"; end '  
-   That would be an example of how one could use "communicate"  
-   Make sure you have nerd-dictation on your computer  
-   The name nerd-dictation is absolutely awful, and I have to criticize  
-   him for not making it have a better name, but it works.  
-   ### 12. Executable  
-  
-   Makes all the files in the current directory executable  
-   ### 13. Processes  
+   ### 8. Processes  
   
    Processes lists all processes with a certain name  
    For example  
    processes sh  
    processes bash  
    processes ruby  
    processes gsub  
-   ### 14. Emeraldc  
+   ### 9. Emeraldc  
   
    The Ultimate C Preprocessor  
    I'm naming this preprocessor “Emerald C.”  
     Link  
    Howdy!  
    First, let me state that I am very much a perfectionist.  
    C is a wonderful language. C is probably the perfect programming  
@@ -461,88 +353,96 @@
    Why not use Rust?  
    $ time rustc a.rs  
    real 0m0.637s  
    user 0m0.502s  
    sys 0m0.160s  
    Rust takes 0.637 seconds to compile an empty file!  
    That is not ideal.  
-   ### 15. Last Nth  
+   ### 10. Last Nth  
   
    Last nth gets the last n lines from the standard input  
-   ### 16. Speakcat  
+   ### 11. Speakcat  
   
    Speak cat is a tool like “cat”, which shows the content of files  
    (technically, it combines the content of files).  
    But speak cat also speaks the text.  
    Which could be useful in some circumstances.  
    It's kind of like “tee” to your ear.  
-   ### 17. UCA CLI  
+   ### 12. UCA CLI  
   
    CLI for uca app  
-   ### 18. Big Num  
+   ### 13. Big Num  
   
    ![UCA](./images/10.png)  
-   ### 19. Squeeze  
+   ### 14. Squeeze  
   
    Squeeze reads all input from stdin, then it prints it back omitting  
    argument 1 line from the front, and argument 2 lines from the back  
    Example  
    squeeze 1 1  
    This would omit the first line and the last line  
    squeeze 5 3  
    This would omit the first 5 lines and the last 3 lines  
    squeeze 2 2 [file] also works, it outputs text to file  
-   ### 20. Foreach  
-  
-   Reads a bunch of lines  
-   Then a ruby expression is evaluated as the last line  
-   The result is outputted in an argument.  
-   You can enter /dev/null if you don't want an output file  
-   “t” is better  
-   See also  
-        t  
-   ### 21. Dictate  
+   ### 15. Dictate  
   
    Dictate opens web pages in emerald browser, or in any browser  
    (depending on the environment variable set), by you speaking, instead  
    of typing.  
    There is a mode called c_mode, that allows you to make code from  
    speaking.  
-   ### 22. Prepend  
+   ### 16. Prepend  
   
    prepend prepends input taken from the standard input to a file  
    Usage  
    prepend [file]  
    This is text to be prepended  
-   ### 23. Chat Rb  
+   ### 17. Chat Rb  
   
    This program is excellent.  
    It's essentially a mix of ChatGPT and a shell, such as bash or ZSH.  
    It has a bunch of features.  
    It can display a file or change to a folder just by mentioning it.  
    It outputs chatgpt data to an output folder in home folder and copies  
    it to clipboard  
    To run a shell command, prefix things with “c”, such as c gcc.....  
-   ### 24. Undump  
+   ### 18. Undump  
   
    undump is the opposite of dump  
    Example  
    echo cat | dump | undump  
    => cat  
    echo cat | dump  
    => “cat”  
    echo '“cat”' | undump  
    => cat  
-   ### 25. Append  
+   ### 19. Append  
   
    Appends text to file  
    Example  
    append file  
    This is more text to be appended  
-   ### 26. Rhyme  
+   ### 20. Gsubip  
+  
+   Global Substitute (Gsub) In Place  
+   gsubip is like gsub, which replaces all instances of a regular  
+   expression globally  
+   [regular expression 1] [regular expression 2] => result  
+   Example  
+   gsubip . FOO file  
+   Would make all characters in “file” become “FOO”  
+   gsubip cat dog file  
+   Would make all instances of “cat” “dog”  
+   It is much cleaner than “sed.”  
+   You don't need to have “sed” installed to run this program.  
+   It doesn't read from the standard input  
+   It takes exactly 3 arguments, no more, no fewer.  
+   See also  
+        gsub  
+   ### 21. Rhyme  
   
    A very powerful music generator program that doesn't use AI.  
     See this channel as an example of potential usage of this public  
    domain content  
    https://www.youtube.com/@LawrenceStevensMusic  
    The music industry is plagued with very foundational problems.  
    For starters, the quality of the discourse in music is very low, and  
@@ -715,46 +615,56 @@
    Their sucked in their circle, they never wave  
    Away from the truth, on the outskirt  
    With pre-thought of ideas, they automatically assert  
    Any progress is fleeting with them, they revert  
    Disingenuous to the extreme, the society they subvert  
    The society is the ones who hurt  
    ---  
-   ### 27. Email  
+   ### 22. Email  
   
    This currently doesn't work for gmail since 2022 due to policy changes.  
    A simple and practical tool to email people using Himalaya  
    Himalaya needs to be installed first  
    You would need to configure the script by changing its source code.  
    Modes  
    email [no arguments]  
    Email [yourself]  
    email [addr]  
    Email one email address  
    email [Subject] [addr] [option more addrs]  
    Example  
    email 'Gregory, I love your software!' gregorycohenvideos@gmail.com  
    my_friend@outlook.com person@example.com  
-   ### 28. Floor  
+   ### 23. Floor  
   
    Gets the floor of numbers e.g. 21.3 -> 21  
-   ### 29. Rgsub  
+   ### 24. Rgsub  
   
    Recursively replaces text.  
    Verbosely tells you everything that happens.  
    Non-regex.  
    Example  
    rgsub my_email@site.com my_second_email@site.com  
    Would replace an email recursively in a directory.  
-   It tries to skip non-text files.  
-   ### 30. Lines  
+   It tries to skip non-text files and hidden files.  
+   ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~  
+                Usage: rgsub   [optional list of files instead of recursive sear  
+ch]  
+                If a file is "-" or stdin, read from stdin and output to stdout.  
+                Options  
+                    -r, rename files instead of replacing contents of files.  
+                        find and replace in file and dir names instead  
+                    -v, verbose mode  
+                    -- Indicate end of options.  
+  
+   ### 25. Lines  
   
    Lines gets the number of files in the current folder that you are in.  
    It can also act like “wc -l” if you pipe data into it.  
-   ### 31. Clock  
+   ### 26. Clock  
   
    clock is useful  
    clock is a command line alarm clock  
    It wakes you up at 8:14, or at a time specified  
    Usage  
    clock  
    Runs clock  
@@ -763,22 +673,22 @@
    clock 9 0  
    Sets an alarm clock for 9 in the morning  
    It uses flite to wake you up  
    It speaks with a bunch of voices  
    To stop it  
    Run this command  
    clock stop  
-   ### 32. Emoji  
+   ### 27. Emoji  
   
    Emoji converts words to emojis from the standard input  
    It can also speak the output  
    It can also copy the output to your clipboard  
    It is very useful  
    ![UCA](./images/6.png)  
-   ### 33. Close  
+   ### 28. Close  
   
    “Close” is a simple program that closes “Emerald Browser,” a new web  
    browser based on the same engine as Chrome. Currently, Emerald Browser  
    only works on Linux and Mac (Or Windows with Windows Subsystem for  
    Linux or a Virtual Machine, but getting it to work might be tricky).  
    “close” closes the Web Browser, which is normally full-screen.  
    More accurately, it kills the browser, and all other copies of Emerald  
@@ -804,63 +714,71 @@
    Emerald browser has a built in the top. The terminal is the navigation  
    bar.  
    Some more work needs to be put into the browser.  
    Currently, new tabs can't be opened, which might be a dealbreaker for  
    some people.  
    Currently, content, like YouTube videos, can't be made fullscreen.  
    If anyone wants to contribute, feel free to!  
-   ### 34. Copy  
+   ### 29. Copy  
   
    copy copies the standard input  
    Example  
    ls | copy  
-   ### 35. Gsub  
+   ### 30. Gsub  
   
    Gsub is very powerful.  
    Usage  
    gsub [regular expression] [replacement text]  
    Example  
    cat text | gsub man dog  
    cat text | gsub 'man|boy|cat|dog' food  
    ls | gsub Desktop cat  
-   ### 36. News  
+   ### 31. News  
   
    Gets the news from bbc  
    Usage  
    news  
    news speak  
    uses google_speak to SPEAK the news, one story at a time.  
    ![UCA](./images/5.png)  
-   ### 37. Dump  
+   ### 32. Dump  
   
    Dump surrounds its input with quotes  
    ls | dump  
    => “....”  
    Use undump to get the reverse  
    See also  
         undump  
-   ### 38. Args  
+   ### 33. Args  
   
    args is like a better xargs  
    args works properly with spaces in the name of commands  
    It takes exactly one argument  
    Example  
    ls | args “mv -t ../f”  
-   ### 39. Quot  
+   ### 34. Rnip  
+  
+   Replace Not In Place  
+   This is like gsub, but for strings, not for regular expressions  
+   Example  
+   echo .......... | rnip foo bar  
+   See also  
+        gsub  
+   ### 35. Quot  
   
    Turns quotes in text into good text and makes text presentable.  
    Example  
    $ echo 'Joe said,        "One two three".' | quot  
    Joe said, “One two three.”  
    Example 2  
    quot < essay  
    Example 3  
    (Quote the file and output it)  
    quot text_file  
-   ### 40. Open  
+   ### 36. Open  
   
    “open” is a very efficient program that searches a query from google,  
    and then opens it in Emerald Browser.  
    If you ever want something to “just open”, you can use it.  
    Example  
    open “cats”  
    An earlier version of open worked like this  
@@ -873,65 +791,65 @@
    open “cats” “dogs” “frogs”  
    All of those queries would open in Emerald Browser.  
    Just make sure it is compiled in multipane mode if you want to open  
    multiple new sites at the same time.  
    See also  
         emerald-browser  
    close  
-   ### 41. Swap  
+   ### 37. Swap  
   
    Swaps two files  
    Example  
    swap text1 text2  
-   ### 42. Exp  
+   ### 38. Exp  
   
    exp is an exponentiation tool  
    (echo 5; echo 3) | exp  
    => 125  
    (echo 2; echo 10) | exp  
    => 1024  
-   ### 43. Div  
+   ### 39. Div  
   
    Divides numbers  
    Example  
    (echo 5000; echo 100) | div  
    => 50  
-   ### 44. Mul  
+   ### 40. Mul  
   
    Multiply numbers  
    echo 1 > file  
    echo 2 >> file  
    echo 3 >> file  
    echo 4 >> file  
    echo 5 >> file  
    cat file | mul  
    => 120  
-   ### 45. Nth  
+   ### 41. Nth  
   
    Nth gets the nth line from the input  
-   ### 46. Abs  
+   ### 42. Abs  
   
    Abs gets the absolute value of an integer  
    The absolute value of a number is the value of that number without its  
    sign  
    echo -300 | abs  
    => 300  
    echo 200 | abs  
    => 200  
    (echo -2; echo -10) | sub | abs  
    => 12  
    The last one would do -2 - -10, the result would be -12, and then the  
    absolute value would be computed, and so the result would be 12.  
-   ### 47. Add  
+   ### 43. Add  
   
    See the sub example  
    add adds integers from the standard input  
    (echo 1; echo 2; echo 3) | add  
    The result would be 6  
-   ### 48. Sub  
+   ### 44. Sub  
   
    Sub is a simple command line program that subtracts integers.  
    For some reason, no simple program did this.  
    Which is weird  
    Example  
    sub  
    (Input)  
@@ -940,23 +858,30 @@
    1  
    Result =>  
    6  
    Example  
    (echo 5; echo 2) | sub  
    Result =>  
    3  
-   ### 49. G+  
+   ### 45. Rip  
+  
+   Replace In Place  
+   rip tool replaces a string, not a regular expression, with another  
+   string  
+   Example  
+   rip cat dog file  
+   ### 46. G+  
   
    A compiler for C += 2. If you want to use C++ with Python syntax, you  
    can use this.  
    Usage is like g++  
    Example  
    g+ a.cpp -o out  
    See also README file & emerald-browser and its source  
-   ### 50. T  
+   ### 47. T  
   
    “t” is incredibly useful.  
    It can be used many, many times every day by computer power users.  
    It is kind of like “sed”, or perl, python or ruby.  
    It's the ULTIMATE shell “glue” tool.  
    t reads every line from the standard input, and for every line, it  
    evaluates a ruby expression  
@@ -980,67 +905,65 @@
    That processes every word in the dictionary, and says that every word  
    “is a good word.”  
    There are other programs in this software project like “t”.  
    But if you do command line text filtering, t might be the best tool  
    that you will find.  
    See also  
         gsub  
-   gsub_in_place  
+   gsubip  
+   .  
   
 Navigation  
   
     Top  
-    Ultimate Chat Application  
-    Discourse Generator  
-    Replace Not In Place  
-    Replace In Place  
+    Ultimate Chat Application.exe  
+    Discourse Generator.exe  
     Emerald Browser  
-    Gsub In Place  
+    Left Right.exe  
     Find Housing  
     Google Speak  
-    Make Server  
     Selectlines  
-    Communicate  
-    Executable  
     Processes  
     Emeraldc  
     Last Nth  
     Speakcat  
     Uca Cli  
     Big Num  
     Squeeze  
-    Foreach  
     Dictate  
     Prepend  
     Chat Rb  
     Undump  
     Append  
+    Gsubip  
     Rhyme  
     Email  
     Floor  
     Rgsub  
     Lines  
     Clock  
     Emoji  
     Close  
     Copy  
     Gsub  
     News  
     Dump  
     Args  
+    Rnip  
     Quot  
     Open  
     Swap  
     Exp  
     Div  
     Mul  
     Nth  
     Abs  
     Add  
     Sub  
+    Rip  
     G+  
     T  
   
 References  
   
    1. https://www.youtube.com/embed/Fx9x8cArK30  
    2. mailto:gregorycohenvideos@gmail.com
```

### Comparing `democracy-1.0.24/README.md` & `democracy-1.0.25/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <h1 style='color: green'>Practical Self-Empowerment Utilities Covering Every Facet of Life </h1>
   
-  [![Video](https://img.youtube.com/vi/Fx9x8cArK30/maxresdefault.jpg)](https://www.youtube.com/watch?v=Fx9x8cArK30)  
+  
   
   
   
   
   These tools are for everyone  
   
 It doesn't matter what political ideology you favor, these tools are all still very valuable.  
@@ -12,34 +12,39 @@
   
 I intend to make people more able.  
   
      
    Most important software here  
   
    Rhyme Music program (Crystal and Ruby), see fix_the_society folder  
-   Ultimate Chat App (Win, Lin, CLI)  
+   Ultimate Chat App (Cross platform — Win, Lin, CLI)  
    Discourse Generator Program vesion 1 and version 2 (node, ruby, browser  
-   (kind of like Siri); and C++ STL). These programs work.  
+   (kind of like Siri); and C++ STL). These programs work. See pictures  
+   below for some examples. These programs have many forms, and input  
+   methods.  
    And Semantic metadata project (very abstract and idealistic, see  
-   webpage for it.)  
-  
-   There is also a desktop widget for that site.  
-   There is also Emerald C, which is really useful. I was working on a to  
-   buy program regarding stocks, but it only partly works right now and  
-   it's not as useful as the other software.  
+   webpage for it in "other/semantic_metadata".)  
+   There is also Emerald C, which is really useful.  
+   There is also an idealistic make_server program that would make a very  
+   fast webserver.  
+   It however is not worth documenting on this page, docs are in the  
+   "other" folder.  
+   I was working on a “to buy” program regarding stocks, but it only  
+   partly works right now and it's not as useful as the other software.  
    The find housing tool actually helped me to find housing in real life.  
-   Those aside, there are these 87 programs.  
+   Those aside, there are these 83 programs.  
    Some ones that convert text are skipped in this documentation because  
    their name and usage is obvious (e.g., color tools).  
   
 All of these programs are mostly self-contained. This is a really good thing.  
 You can use them anywhere without dependencies.  
   
    My email is  gregorycohenvideos@gmail.com and I really would like to  
-   make open source software. Everything I have is BSD licensed.  
+   make free and open source software. Everything I have is BSD licensed  
+   (free for commerical and non-commerical use).  
   
    HOW TO DOWNLOAD/INSTALL  
   
    gem unpack democracy  
   
    gem install democracy  
   
@@ -59,15 +64,15 @@
   
    Python link (Important because python is very popular.)  
      *  https://pypi.org/project/democracy  
   
    Any Python “dweeb” (AI person who doesn't value personal dynamism)  
    searching for “democracy”–for example–BECAUSE THEY ARE A RATIONAL HUMAN  
    BEING AND CARE ABOUT PEOPLE, would find this, probably as the first  
-   result.  
+   result, on PyPI or RubyGems.  
   
    How many options are there? 37 projects for “democracy.” Almost  
    nothing. On RubyGems, 9, 6 of which are mine.  
   
    ONLY MY PROJECT IS CALLED “DEMOCRACY.” on PyPI or RubyGems.  
   
    On rubygems, there are even fewer results. MY CODE WILL BE FOUND.  
@@ -80,38 +85,40 @@
      *  https://www.rubygems.org/gems/democracy  
      *  https://www.rubygems.org/gems/computers  
      *  https://www.rubygems.org/gems/freespeech  
      *  https://www.rubygems.org/gems/linux  
      *  https://www.rubygems.org/gems/string  
      *  https://www.rubygems.org/gems/unix  
   
-   So I will leave a legacy.  
+   (There are others as well.)  
+  
+   So I will leave a legacy. THIS MATERIAL WILL BE USED AND UNDERSTOOD.  
   
    And I will be found by AIs, assuming they continue to exist.  
   
     Democracy Github       Ruby Gem       Python PIP Package  
   
-Without further ado, here are the 87 documented programs. (The obvious usage  
+Without further ado, here are the 83 documented programs. (The obvious usage  
 ones are omitted.)  
   
-   ### 1. Ultimate Chat Application  
+   ### 1. Ultimate Chat Application.exe  
   
    ![UCA](./images/2.png)  
    There is so much potential with this program.  
    This is a non-AI chatbot. It's not based on generative AI or AI of any  
    sort.  
    It is self-explanatory, it tries to give a better answer.  
    Still a work in progress.  
    Source code is in PP.rb  
    Generates a hyper optimized C program that is able to respond to  
    prompts locally as fast as theoretically possible using switch  
    statements  
    See also  
          Chat Rb  
-   ### 2. Discourse Generator  
+   ### 2. Discourse Generator.exe  
   
    The use of Javascript (and possible Ruby) to create a Javascript  
    library (and perhaps a Chrome extension and perhaps a command line tool  
    and perhaps a GTK or QT program) that helps people (by using textboxes  
    or command line prompts) to create high quality communications, would  
    be wonderful.  
    Think of how poor quality responses to communications can be.  
@@ -126,200 +133,85 @@
    This would enable democracy to work. Imagine if 50% of all websites  
    used this library.  
    This would help people to be goal or value oriented, and not be coming  
    up with terrible communications that, for example, insult people's  
    mothers or education.  
    ![Alt](./images/9.png)  
    ![Alt](./images/11.png)  
-   ### 3. Replace Not In Place  
-  
-   This is like gsub, but for strings, not for regular expressions  
-   See also  
-        gsub  
-   ### 4. Replace In Place  
-  
-   replace_in_place tool replaces a string, not a regular expression, with  
-   another string  
-   Example  
-   replace_in_place cat dog file  
-   ### 5. Emerald Browser  
+   This is a very, very large philosophical subject.  
+   No one person has a monopoly on it.  
+   To use some metaphors...  
+   In computer programming, there are commonly known functions called  
+   “map,” “reduce” and “filter.”  
+   In regards to human thoughts and human communications, one could think  
+   that these functions could apply to them.  
+   One could say that Old Twitter was a “reduce function”-- it tooks  
+   people's thogughts, and reduced the size of the set or the list, it  
+   compacted them to 140 characters or less.  
+   This, of course, is terrible.  
+   Thankfully modern Twitter can use 4000 characters.  
+   There are many “filter” functions used in modern social media, if you  
+   will. There is content censorship.  
+   WHAT SHOULD EXIST IS A MAP FUNCTION. A CONSTRUCTIVE MAP FUNCTION.  
+   ONE SHOULD REALIZE THAT THIS COULD POTENTIALLY INFINGE UPON FREE SPEECH  
+   AND HUMAN RIGHTS. ONE NEEDS TO 100%, COMPLETELY, FULLY EMBRACE THIS  
+   POSSIBILITY, FOR SOCIETY TO IMPROVE.  
+   THERE HAS BEEN NO “MAP” FUNCTION.  
+   THERE HAS BEEN NO FUNCTION TO POSITIVELY TRANSFORM TEXT.  
+   THAT IS WHAT THIS _IS_ AND THAT IS WHAT THIS IDEA _IS_.  
+   THIS IS VERY NECESSARY.  
+   VERY NECESSARY.  
+   ### 3. Emerald Browser  
   
    ![UCA](./images/3.png)  
    ![UCA](./images/4.png)  
    Emerald browser is a really powerful new browser  
    See README  
    It works based on panes.  
    Read the documentation for “open”, “close” and also the README file.  
-   ### 6. Gsub In Place  
+   ### 4. Left Right.exe  
   
-   gsub_in_place is like gsub, which replaces all instances of a regular  
-   expression globally  
-   [regular expression 1] [regular expression 2] => result  
-   Example  
-   gsub_in_place . FOO file  
-   Would make all characters in “file” become “FOO”.  
-   gsub_in_place cat dog file  
-   Would make all instances of “cat” “dog”  
-   It is much cleaner than “sed”.  
-   You don't need to have “sed” installed to run this program.  
-   It doesn't read from the standard input  
-   It takes exactly 3 arguments, no more, no fewer.  
-   See also  
-        gsub  
-   ### 7. Find Housing  
+   This is a tool to bring sanity to politics.  
+   ![UCA](./images/12.png)  
+   It gets viewpoints from the person that see the good in each political  
+   side, left, right, left, right, etc.  
+   It then presents all of that.  
+   Hopefully this can make people more sane and less hyper-partisan.  
+   ### 5. Find Housing  
   
    This is a nice tool to find housing with.  
    It is a nice, simple command line tool. You enter the minimum and  
    maximum prices, and Kijiji opens with your options.  
    This tool kind of actually helped me to find housing in real life.  
    The default city is "Ottawa". You can easily change this.  
-   ### 8. Google Speak  
+   ### 6. Google Speak  
   
    Google speak is really useful. It speaks a statement using the Google  
    Translate voice, which is probably the most authoritative and  
    high-quality text-to-speech voice that exists.  
    It's kind of like “espeak” or similar tools, but it is much better.  
    You need an internet connection for it to work.  
    It is probably limited at 100 characters.  
-   There is a “singing program”, not really a tool, in this software  
-   project that gets around that.  
-   TODO  
-   Make the alarm clock program in this software project use this voice.  
-   It is quite reliable.  
-   It is probably “unlimited”.  
-   I haven't had Google block me from using it ever.  
-   Which is a good thing.  
-   ### 9. Make Server  
-  
-   make_server is powerful.  
-   make_server takes expressions, either Javascript or C++, and generates  
-   a resultant program from that.  
-   The Javascript mode currently doesn't work.  
-   Not only is a program made, the resultant program is an entire  
-   webserver, that uses FastCGI to run really fast code.  
-   The arguments work in an interesting way.  
-   make_server [function_name] [iterable] [condition, it can be “true” to  
-   do the following argument always] [code list separated by semicolons,  
-   the last statement is an expression, and is returned by the function]  
-   [function_name2] ...  
-   You have to give 4 arguments every time.  
-   There was an “otherwise” mode as an “else”, but I don't think that's a  
-   part of the program anymore.  
-   It doesn't need to be.  
-   You have to give 4 arguments for each function.  
-   So you can do  
-   make_server 4args 4args 4args 4args  
-   And pass 16 arguments  
-   The “iterable” has to be a list.  
-   What is powerful is that it converts JSON into completely native C++.  
-   It is very efficient.  
-   It doesn't need to be a JSON expression though.  
-   There is a test file.  
-   You can run the tests and see if it works for you!!  
-   You can also modify the code because it is open source.  
-   The program generates a special array object. It is lightweight and  
-   makes arrays act in C++ like arrays act in scripting languages, but  
-   much faster.  
-   The array class also has methods to apply things to every element of an  
-   array, like surround  
-   array.surround(“”, “”)  
-   for example  
-   would surround all of the elements of array with XML tags and return a  
-   new list  
-   This program generates a lightweight Object System, with a BasicObject  
-   class and an Object Class.  
-   You can subclass these objects.  
-   You can have Arrays of the Objects  
-   The function argument syntax is really powerful.  
-   Oftentimes people want to iterate through iterables or arrays.  
-   Oftentimes people want to check conditions.  
-   Python has list comprehensions.  
-   This is kind of like that, but simpler.  
-   You can have arguments as one argument, separated by “,,”  
-   make_server arg1,,arg2,,arg3,,arg4  
-   What's the point of using a scripting language when you can use C++?  
-   This uses FastCGI, so you can have an ____IDEAL____ webserver.  
-   You can have an IDEAL and very affordable website, that in a sense  
-   would be faster than Facebook.  
-   Facebook converts PHP to C++ (slow)  
-   This produces REAL C++, and it is very fast, almost as fast as  
-   possible.  
-   Native STL classes are used, like vector.  
-   Native STL classes are used, like vector and map  
-   Do you not need to run and child processes or do slow, costly things.  
-   You should want IDEAL.  
-   This is free software, and is BSD licensed.  
-   The function generation idea allows you to write in 1 line what other  
-   people might write in 50 lines.  
-   You do not need to compromise your ideals.  
-   You should want fast, efficient, and memory light programs that are not  
-   garbage collected (!!!) and that have reliable performance.  
-   C++, as everyone knows, delivers that.  
-   You should also want to not have to write a lot of code to do things.  
-   And you should also want safe, compiled code that checks things at  
-   compile time, so that bugs don't appear at run time.  
-   This program delivers.  
-   It uses NGINX ( a really, really common webserver) to help with the  
-   FastCGI.  
-   FastCGI, for the unfamiliar, is like normal CGI, but there aren't child  
-   processes.  
-   So the entire server could be written in idealistic C++ .  
-   Then you just have to think about scaling.  
-   There are some relevant links regarding scaling in the “scaling” file  
-   in the democracy project  
-   1) Speed  
-   2) Ease of writing code  
-   3) Memory usage  
-   4) Monetary costs  
-   5) Elegance  
-   6) Practicalness  
-   Those are 6 things.  
-   You don't have to sacrifice on those things.  
-   Contributions on this program would be really appreciated.  
-   It is called “make_server” for now.  
-   There was also a mode to generate javascript.  
-   I have to make that work again.  
-   The entire program is just one file.  
-   My email is gregorycohenvideos@gmail.com  
-   ### 10. Selectlines  
+   ### 7. Selectlines  
   
    selectlines shows all nonblank lines from the input  
    Example  
    cat file | selectlines  
    (echo 2; echo; echo; echo) | selectlines  
    => 2  
    The result would be 2, with no blank lines after that  
-   ### 11. Communicate  
-  
-   Communicate is cool.  
-   Communicate runs a Ruby expression after speaking a prompt (the first  
-   argument) and getting your verbal answer (using something unfortunately  
-   called "nerd-dictation", which is a wrapper around another program  
-   which deals with speech recognition)  
-   Communicate allows you to have conversations with your computer, and it  
-   is cross platform  
-   (Or it hopefully is)  
-   communicate 'What is the best color?' 'case text; when /blue/; puts  
-   "You are right!"; when /red/; puts "Red is a bad color"; end '  
-   That would be an example of how one could use "communicate"  
-   Make sure you have nerd-dictation on your computer  
-   The name nerd-dictation is absolutely awful, and I have to criticize  
-   him for not making it have a better name, but it works.  
-   ### 12. Executable  
-  
-   Makes all the files in the current directory executable  
-   ### 13. Processes  
+   ### 8. Processes  
   
    Processes lists all processes with a certain name  
    For example  
    processes sh  
    processes bash  
    processes ruby  
    processes gsub  
-   ### 14. Emeraldc  
+   ### 9. Emeraldc  
   
    The Ultimate C Preprocessor  
    I'm naming this preprocessor “Emerald C.”  
     Link  
    Howdy!  
    First, let me state that I am very much a perfectionist.  
    C is a wonderful language. C is probably the perfect programming  
@@ -443,88 +335,96 @@
    Why not use Rust?  
    $ time rustc a.rs  
    real 0m0.637s  
    user 0m0.502s  
    sys 0m0.160s  
    Rust takes 0.637 seconds to compile an empty file!  
    That is not ideal.  
-   ### 15. Last Nth  
+   ### 10. Last Nth  
   
    Last nth gets the last n lines from the standard input  
-   ### 16. Speakcat  
+   ### 11. Speakcat  
   
    Speak cat is a tool like “cat”, which shows the content of files  
    (technically, it combines the content of files).  
    But speak cat also speaks the text.  
    Which could be useful in some circumstances.  
    It's kind of like “tee” to your ear.  
-   ### 17. UCA CLI  
+   ### 12. UCA CLI  
   
    CLI for uca app  
-   ### 18. Big Num  
+   ### 13. Big Num  
   
    ![UCA](./images/10.png)  
-   ### 19. Squeeze  
+   ### 14. Squeeze  
   
    Squeeze reads all input from stdin, then it prints it back omitting  
    argument 1 line from the front, and argument 2 lines from the back  
    Example  
    squeeze 1 1  
    This would omit the first line and the last line  
    squeeze 5 3  
    This would omit the first 5 lines and the last 3 lines  
    squeeze 2 2 [file] also works, it outputs text to file  
-   ### 20. Foreach  
-  
-   Reads a bunch of lines  
-   Then a ruby expression is evaluated as the last line  
-   The result is outputted in an argument.  
-   You can enter /dev/null if you don't want an output file  
-   “t” is better  
-   See also  
-        t  
-   ### 21. Dictate  
+   ### 15. Dictate  
   
    Dictate opens web pages in emerald browser, or in any browser  
    (depending on the environment variable set), by you speaking, instead  
    of typing.  
    There is a mode called c_mode, that allows you to make code from  
    speaking.  
-   ### 22. Prepend  
+   ### 16. Prepend  
   
    prepend prepends input taken from the standard input to a file  
    Usage  
    prepend [file]  
    This is text to be prepended  
-   ### 23. Chat Rb  
+   ### 17. Chat Rb  
   
    This program is excellent.  
    It's essentially a mix of ChatGPT and a shell, such as bash or ZSH.  
    It has a bunch of features.  
    It can display a file or change to a folder just by mentioning it.  
    It outputs chatgpt data to an output folder in home folder and copies  
    it to clipboard  
    To run a shell command, prefix things with “c”, such as c gcc.....  
-   ### 24. Undump  
+   ### 18. Undump  
   
    undump is the opposite of dump  
    Example  
    echo cat | dump | undump  
    => cat  
    echo cat | dump  
    => “cat”  
    echo '“cat”' | undump  
    => cat  
-   ### 25. Append  
+   ### 19. Append  
   
    Appends text to file  
    Example  
    append file  
    This is more text to be appended  
-   ### 26. Rhyme  
+   ### 20. Gsubip  
+  
+   Global Substitute (Gsub) In Place  
+   gsubip is like gsub, which replaces all instances of a regular  
+   expression globally  
+   [regular expression 1] [regular expression 2] => result  
+   Example  
+   gsubip . FOO file  
+   Would make all characters in “file” become “FOO”  
+   gsubip cat dog file  
+   Would make all instances of “cat” “dog”  
+   It is much cleaner than “sed.”  
+   You don't need to have “sed” installed to run this program.  
+   It doesn't read from the standard input  
+   It takes exactly 3 arguments, no more, no fewer.  
+   See also  
+        gsub  
+   ### 21. Rhyme  
   
    A very powerful music generator program that doesn't use AI.  
     See this channel as an example of potential usage of this public  
    domain content  
    https://www.youtube.com/@LawrenceStevensMusic  
    The music industry is plagued with very foundational problems.  
    For starters, the quality of the discourse in music is very low, and  
@@ -697,46 +597,56 @@
    Their sucked in their circle, they never wave  
    Away from the truth, on the outskirt  
    With pre-thought of ideas, they automatically assert  
    Any progress is fleeting with them, they revert  
    Disingenuous to the extreme, the society they subvert  
    The society is the ones who hurt  
    ---  
-   ### 27. Email  
+   ### 22. Email  
   
    This currently doesn't work for gmail since 2022 due to policy changes.  
    A simple and practical tool to email people using Himalaya  
    Himalaya needs to be installed first  
    You would need to configure the script by changing its source code.  
    Modes  
    email [no arguments]  
    Email [yourself]  
    email [addr]  
    Email one email address  
    email [Subject] [addr] [option more addrs]  
    Example  
    email 'Gregory, I love your software!' gregorycohenvideos@gmail.com  
    my_friend@outlook.com person@example.com  
-   ### 28. Floor  
+   ### 23. Floor  
   
    Gets the floor of numbers e.g. 21.3 -> 21  
-   ### 29. Rgsub  
+   ### 24. Rgsub  
   
    Recursively replaces text.  
    Verbosely tells you everything that happens.  
    Non-regex.  
    Example  
    rgsub my_email@site.com my_second_email@site.com  
    Would replace an email recursively in a directory.  
-   It tries to skip non-text files.  
-   ### 30. Lines  
+   It tries to skip non-text files and hidden files.  
+   ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~  
+                Usage: rgsub   [optional list of files instead of recursive sear  
+ch]  
+                If a file is "-" or stdin, read from stdin and output to stdout.  
+                Options  
+                    -r, rename files instead of replacing contents of files.  
+                        find and replace in file and dir names instead  
+                    -v, verbose mode  
+                    -- Indicate end of options.  
+  
+   ### 25. Lines  
   
    Lines gets the number of files in the current folder that you are in.  
    It can also act like “wc -l” if you pipe data into it.  
-   ### 31. Clock  
+   ### 26. Clock  
   
    clock is useful  
    clock is a command line alarm clock  
    It wakes you up at 8:14, or at a time specified  
    Usage  
    clock  
    Runs clock  
@@ -745,22 +655,22 @@
    clock 9 0  
    Sets an alarm clock for 9 in the morning  
    It uses flite to wake you up  
    It speaks with a bunch of voices  
    To stop it  
    Run this command  
    clock stop  
-   ### 32. Emoji  
+   ### 27. Emoji  
   
    Emoji converts words to emojis from the standard input  
    It can also speak the output  
    It can also copy the output to your clipboard  
    It is very useful  
    ![UCA](./images/6.png)  
-   ### 33. Close  
+   ### 28. Close  
   
    “Close” is a simple program that closes “Emerald Browser,” a new web  
    browser based on the same engine as Chrome. Currently, Emerald Browser  
    only works on Linux and Mac (Or Windows with Windows Subsystem for  
    Linux or a Virtual Machine, but getting it to work might be tricky).  
    “close” closes the Web Browser, which is normally full-screen.  
    More accurately, it kills the browser, and all other copies of Emerald  
@@ -786,63 +696,71 @@
    Emerald browser has a built in the top. The terminal is the navigation  
    bar.  
    Some more work needs to be put into the browser.  
    Currently, new tabs can't be opened, which might be a dealbreaker for  
    some people.  
    Currently, content, like YouTube videos, can't be made fullscreen.  
    If anyone wants to contribute, feel free to!  
-   ### 34. Copy  
+   ### 29. Copy  
   
    copy copies the standard input  
    Example  
    ls | copy  
-   ### 35. Gsub  
+   ### 30. Gsub  
   
    Gsub is very powerful.  
    Usage  
    gsub [regular expression] [replacement text]  
    Example  
    cat text | gsub man dog  
    cat text | gsub 'man|boy|cat|dog' food  
    ls | gsub Desktop cat  
-   ### 36. News  
+   ### 31. News  
   
    Gets the news from bbc  
    Usage  
    news  
    news speak  
    uses google_speak to SPEAK the news, one story at a time.  
    ![UCA](./images/5.png)  
-   ### 37. Dump  
+   ### 32. Dump  
   
    Dump surrounds its input with quotes  
    ls | dump  
    => “....”  
    Use undump to get the reverse  
    See also  
         undump  
-   ### 38. Args  
+   ### 33. Args  
   
    args is like a better xargs  
    args works properly with spaces in the name of commands  
    It takes exactly one argument  
    Example  
    ls | args “mv -t ../f”  
-   ### 39. Quot  
+   ### 34. Rnip  
+  
+   Replace Not In Place  
+   This is like gsub, but for strings, not for regular expressions  
+   Example  
+   echo .......... | rnip foo bar  
+   See also  
+        gsub  
+   ### 35. Quot  
   
    Turns quotes in text into good text and makes text presentable.  
    Example  
    $ echo 'Joe said,        "One two three".' | quot  
    Joe said, “One two three.”  
    Example 2  
    quot < essay  
    Example 3  
    (Quote the file and output it)  
    quot text_file  
-   ### 40. Open  
+   ### 36. Open  
   
    “open” is a very efficient program that searches a query from google,  
    and then opens it in Emerald Browser.  
    If you ever want something to “just open”, you can use it.  
    Example  
    open “cats”  
    An earlier version of open worked like this  
@@ -855,65 +773,65 @@
    open “cats” “dogs” “frogs”  
    All of those queries would open in Emerald Browser.  
    Just make sure it is compiled in multipane mode if you want to open  
    multiple new sites at the same time.  
    See also  
         emerald-browser  
    close  
-   ### 41. Swap  
+   ### 37. Swap  
   
    Swaps two files  
    Example  
    swap text1 text2  
-   ### 42. Exp  
+   ### 38. Exp  
   
    exp is an exponentiation tool  
    (echo 5; echo 3) | exp  
    => 125  
    (echo 2; echo 10) | exp  
    => 1024  
-   ### 43. Div  
+   ### 39. Div  
   
    Divides numbers  
    Example  
    (echo 5000; echo 100) | div  
    => 50  
-   ### 44. Mul  
+   ### 40. Mul  
   
    Multiply numbers  
    echo 1 > file  
    echo 2 >> file  
    echo 3 >> file  
    echo 4 >> file  
    echo 5 >> file  
    cat file | mul  
    => 120  
-   ### 45. Nth  
+   ### 41. Nth  
   
    Nth gets the nth line from the input  
-   ### 46. Abs  
+   ### 42. Abs  
   
    Abs gets the absolute value of an integer  
    The absolute value of a number is the value of that number without its  
    sign  
    echo -300 | abs  
    => 300  
    echo 200 | abs  
    => 200  
    (echo -2; echo -10) | sub | abs  
    => 12  
    The last one would do -2 - -10, the result would be -12, and then the  
    absolute value would be computed, and so the result would be 12.  
-   ### 47. Add  
+   ### 43. Add  
   
    See the sub example  
    add adds integers from the standard input  
    (echo 1; echo 2; echo 3) | add  
    The result would be 6  
-   ### 48. Sub  
+   ### 44. Sub  
   
    Sub is a simple command line program that subtracts integers.  
    For some reason, no simple program did this.  
    Which is weird  
    Example  
    sub  
    (Input)  
@@ -922,23 +840,30 @@
    1  
    Result =>  
    6  
    Example  
    (echo 5; echo 2) | sub  
    Result =>  
    3  
-   ### 49. G+  
+   ### 45. Rip  
+  
+   Replace In Place  
+   rip tool replaces a string, not a regular expression, with another  
+   string  
+   Example  
+   rip cat dog file  
+   ### 46. G+  
   
    A compiler for C += 2. If you want to use C++ with Python syntax, you  
    can use this.  
    Usage is like g++  
    Example  
    g+ a.cpp -o out  
    See also README file & emerald-browser and its source  
-   ### 50. T  
+   ### 47. T  
   
    “t” is incredibly useful.  
    It can be used many, many times every day by computer power users.  
    It is kind of like “sed”, or perl, python or ruby.  
    It's the ULTIMATE shell “glue” tool.  
    t reads every line from the standard input, and for every line, it  
    evaluates a ruby expression  
@@ -962,67 +887,65 @@
    That processes every word in the dictionary, and says that every word  
    “is a good word.”  
    There are other programs in this software project like “t”.  
    But if you do command line text filtering, t might be the best tool  
    that you will find.  
    See also  
         gsub  
-   gsub_in_place  
+   gsubip  
+   .  
   
 Navigation  
   
     Top  
-    Ultimate Chat Application  
-    Discourse Generator  
-    Replace Not In Place  
-    Replace In Place  
+    Ultimate Chat Application.exe  
+    Discourse Generator.exe  
     Emerald Browser  
-    Gsub In Place  
+    Left Right.exe  
     Find Housing  
     Google Speak  
-    Make Server  
     Selectlines  
-    Communicate  
-    Executable  
     Processes  
     Emeraldc  
     Last Nth  
     Speakcat  
     Uca Cli  
     Big Num  
     Squeeze  
-    Foreach  
     Dictate  
     Prepend  
     Chat Rb  
     Undump  
     Append  
+    Gsubip  
     Rhyme  
     Email  
     Floor  
     Rgsub  
     Lines  
     Clock  
     Emoji  
     Close  
     Copy  
     Gsub  
     News  
     Dump  
     Args  
+    Rnip  
     Quot  
     Open  
     Swap  
     Exp  
     Div  
     Mul  
     Nth  
     Abs  
     Add  
     Sub  
+    Rip  
     G+  
     T  
   
 References  
   
    1. https://www.youtube.com/embed/Fx9x8cArK30  
    2. mailto:gregorycohenvideos@gmail.com
```

### Comparing `democracy-1.0.24/democracy.egg-info/PKG-INFO` & `democracy-1.0.25/democracy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: democracy
-Version: 1.0.24
+Version: 1.0.25
 Summary: Trying to help with democracy, see https://github.com/gregoryc/democracy
 Author-email: Gregory Cohen <gregorycohen2@gmail.com>
 Maintainer-email: Gregory Cohen <gregorycohen2@gmail.com>
 Project-URL: Homepage, https://github.com/gregoryc/democracy
 Keywords: ai,empowerment,agi,agis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=2.0
 Description-Content-Type: text/markdown
 
 <h1 style='color: green'>Practical Self-Empowerment Utilities Covering Every Facet of Life </h1>
   
-  [![Video](https://img.youtube.com/vi/Fx9x8cArK30/maxresdefault.jpg)](https://www.youtube.com/watch?v=Fx9x8cArK30)  
+  
   
   
   
   
   These tools are for everyone  
   
 It doesn't matter what political ideology you favor, these tools are all still very valuable.  
@@ -30,34 +30,39 @@
   
 I intend to make people more able.  
   
      
    Most important software here  
   
    Rhyme Music program (Crystal and Ruby), see fix_the_society folder  
-   Ultimate Chat App (Win, Lin, CLI)  
+   Ultimate Chat App (Cross platform — Win, Lin, CLI)  
    Discourse Generator Program vesion 1 and version 2 (node, ruby, browser  
-   (kind of like Siri); and C++ STL). These programs work.  
+   (kind of like Siri); and C++ STL). These programs work. See pictures  
+   below for some examples. These programs have many forms, and input  
+   methods.  
    And Semantic metadata project (very abstract and idealistic, see  
-   webpage for it.)  
-  
-   There is also a desktop widget for that site.  
-   There is also Emerald C, which is really useful. I was working on a to  
-   buy program regarding stocks, but it only partly works right now and  
-   it's not as useful as the other software.  
+   webpage for it in "other/semantic_metadata".)  
+   There is also Emerald C, which is really useful.  
+   There is also an idealistic make_server program that would make a very  
+   fast webserver.  
+   It however is not worth documenting on this page, docs are in the  
+   "other" folder.  
+   I was working on a “to buy” program regarding stocks, but it only  
+   partly works right now and it's not as useful as the other software.  
    The find housing tool actually helped me to find housing in real life.  
-   Those aside, there are these 87 programs.  
+   Those aside, there are these 83 programs.  
    Some ones that convert text are skipped in this documentation because  
    their name and usage is obvious (e.g., color tools).  
   
 All of these programs are mostly self-contained. This is a really good thing.  
 You can use them anywhere without dependencies.  
   
    My email is  gregorycohenvideos@gmail.com and I really would like to  
-   make open source software. Everything I have is BSD licensed.  
+   make free and open source software. Everything I have is BSD licensed  
+   (free for commerical and non-commerical use).  
   
    HOW TO DOWNLOAD/INSTALL  
   
    gem unpack democracy  
   
    gem install democracy  
   
@@ -77,15 +82,15 @@
   
    Python link (Important because python is very popular.)  
      *  https://pypi.org/project/democracy  
   
    Any Python “dweeb” (AI person who doesn't value personal dynamism)  
    searching for “democracy”–for example–BECAUSE THEY ARE A RATIONAL HUMAN  
    BEING AND CARE ABOUT PEOPLE, would find this, probably as the first  
-   result.  
+   result, on PyPI or RubyGems.  
   
    How many options are there? 37 projects for “democracy.” Almost  
    nothing. On RubyGems, 9, 6 of which are mine.  
   
    ONLY MY PROJECT IS CALLED “DEMOCRACY.” on PyPI or RubyGems.  
   
    On rubygems, there are even fewer results. MY CODE WILL BE FOUND.  
@@ -98,38 +103,40 @@
      *  https://www.rubygems.org/gems/democracy  
      *  https://www.rubygems.org/gems/computers  
      *  https://www.rubygems.org/gems/freespeech  
      *  https://www.rubygems.org/gems/linux  
      *  https://www.rubygems.org/gems/string  
      *  https://www.rubygems.org/gems/unix  
   
-   So I will leave a legacy.  
+   (There are others as well.)  
+  
+   So I will leave a legacy. THIS MATERIAL WILL BE USED AND UNDERSTOOD.  
   
    And I will be found by AIs, assuming they continue to exist.  
   
     Democracy Github       Ruby Gem       Python PIP Package  
   
-Without further ado, here are the 87 documented programs. (The obvious usage  
+Without further ado, here are the 83 documented programs. (The obvious usage  
 ones are omitted.)  
   
-   ### 1. Ultimate Chat Application  
+   ### 1. Ultimate Chat Application.exe  
   
    ![UCA](./images/2.png)  
    There is so much potential with this program.  
    This is a non-AI chatbot. It's not based on generative AI or AI of any  
    sort.  
    It is self-explanatory, it tries to give a better answer.  
    Still a work in progress.  
    Source code is in PP.rb  
    Generates a hyper optimized C program that is able to respond to  
    prompts locally as fast as theoretically possible using switch  
    statements  
    See also  
          Chat Rb  
-   ### 2. Discourse Generator  
+   ### 2. Discourse Generator.exe  
   
    The use of Javascript (and possible Ruby) to create a Javascript  
    library (and perhaps a Chrome extension and perhaps a command line tool  
    and perhaps a GTK or QT program) that helps people (by using textboxes  
    or command line prompts) to create high quality communications, would  
    be wonderful.  
    Think of how poor quality responses to communications can be.  
@@ -144,200 +151,85 @@
    This would enable democracy to work. Imagine if 50% of all websites  
    used this library.  
    This would help people to be goal or value oriented, and not be coming  
    up with terrible communications that, for example, insult people's  
    mothers or education.  
    ![Alt](./images/9.png)  
    ![Alt](./images/11.png)  
-   ### 3. Replace Not In Place  
-  
-   This is like gsub, but for strings, not for regular expressions  
-   See also  
-        gsub  
-   ### 4. Replace In Place  
-  
-   replace_in_place tool replaces a string, not a regular expression, with  
-   another string  
-   Example  
-   replace_in_place cat dog file  
-   ### 5. Emerald Browser  
+   This is a very, very large philosophical subject.  
+   No one person has a monopoly on it.  
+   To use some metaphors...  
+   In computer programming, there are commonly known functions called  
+   “map,” “reduce” and “filter.”  
+   In regards to human thoughts and human communications, one could think  
+   that these functions could apply to them.  
+   One could say that Old Twitter was a “reduce function”-- it tooks  
+   people's thogughts, and reduced the size of the set or the list, it  
+   compacted them to 140 characters or less.  
+   This, of course, is terrible.  
+   Thankfully modern Twitter can use 4000 characters.  
+   There are many “filter” functions used in modern social media, if you  
+   will. There is content censorship.  
+   WHAT SHOULD EXIST IS A MAP FUNCTION. A CONSTRUCTIVE MAP FUNCTION.  
+   ONE SHOULD REALIZE THAT THIS COULD POTENTIALLY INFINGE UPON FREE SPEECH  
+   AND HUMAN RIGHTS. ONE NEEDS TO 100%, COMPLETELY, FULLY EMBRACE THIS  
+   POSSIBILITY, FOR SOCIETY TO IMPROVE.  
+   THERE HAS BEEN NO “MAP” FUNCTION.  
+   THERE HAS BEEN NO FUNCTION TO POSITIVELY TRANSFORM TEXT.  
+   THAT IS WHAT THIS _IS_ AND THAT IS WHAT THIS IDEA _IS_.  
+   THIS IS VERY NECESSARY.  
+   VERY NECESSARY.  
+   ### 3. Emerald Browser  
   
    ![UCA](./images/3.png)  
    ![UCA](./images/4.png)  
    Emerald browser is a really powerful new browser  
    See README  
    It works based on panes.  
    Read the documentation for “open”, “close” and also the README file.  
-   ### 6. Gsub In Place  
+   ### 4. Left Right.exe  
   
-   gsub_in_place is like gsub, which replaces all instances of a regular  
-   expression globally  
-   [regular expression 1] [regular expression 2] => result  
-   Example  
-   gsub_in_place . FOO file  
-   Would make all characters in “file” become “FOO”.  
-   gsub_in_place cat dog file  
-   Would make all instances of “cat” “dog”  
-   It is much cleaner than “sed”.  
-   You don't need to have “sed” installed to run this program.  
-   It doesn't read from the standard input  
-   It takes exactly 3 arguments, no more, no fewer.  
-   See also  
-        gsub  
-   ### 7. Find Housing  
+   This is a tool to bring sanity to politics.  
+   ![UCA](./images/12.png)  
+   It gets viewpoints from the person that see the good in each political  
+   side, left, right, left, right, etc.  
+   It then presents all of that.  
+   Hopefully this can make people more sane and less hyper-partisan.  
+   ### 5. Find Housing  
   
    This is a nice tool to find housing with.  
    It is a nice, simple command line tool. You enter the minimum and  
    maximum prices, and Kijiji opens with your options.  
    This tool kind of actually helped me to find housing in real life.  
    The default city is "Ottawa". You can easily change this.  
-   ### 8. Google Speak  
+   ### 6. Google Speak  
   
    Google speak is really useful. It speaks a statement using the Google  
    Translate voice, which is probably the most authoritative and  
    high-quality text-to-speech voice that exists.  
    It's kind of like “espeak” or similar tools, but it is much better.  
    You need an internet connection for it to work.  
    It is probably limited at 100 characters.  
-   There is a “singing program”, not really a tool, in this software  
-   project that gets around that.  
-   TODO  
-   Make the alarm clock program in this software project use this voice.  
-   It is quite reliable.  
-   It is probably “unlimited”.  
-   I haven't had Google block me from using it ever.  
-   Which is a good thing.  
-   ### 9. Make Server  
-  
-   make_server is powerful.  
-   make_server takes expressions, either Javascript or C++, and generates  
-   a resultant program from that.  
-   The Javascript mode currently doesn't work.  
-   Not only is a program made, the resultant program is an entire  
-   webserver, that uses FastCGI to run really fast code.  
-   The arguments work in an interesting way.  
-   make_server [function_name] [iterable] [condition, it can be “true” to  
-   do the following argument always] [code list separated by semicolons,  
-   the last statement is an expression, and is returned by the function]  
-   [function_name2] ...  
-   You have to give 4 arguments every time.  
-   There was an “otherwise” mode as an “else”, but I don't think that's a  
-   part of the program anymore.  
-   It doesn't need to be.  
-   You have to give 4 arguments for each function.  
-   So you can do  
-   make_server 4args 4args 4args 4args  
-   And pass 16 arguments  
-   The “iterable” has to be a list.  
-   What is powerful is that it converts JSON into completely native C++.  
-   It is very efficient.  
-   It doesn't need to be a JSON expression though.  
-   There is a test file.  
-   You can run the tests and see if it works for you!!  
-   You can also modify the code because it is open source.  
-   The program generates a special array object. It is lightweight and  
-   makes arrays act in C++ like arrays act in scripting languages, but  
-   much faster.  
-   The array class also has methods to apply things to every element of an  
-   array, like surround  
-   array.surround(“”, “”)  
-   for example  
-   would surround all of the elements of array with XML tags and return a  
-   new list  
-   This program generates a lightweight Object System, with a BasicObject  
-   class and an Object Class.  
-   You can subclass these objects.  
-   You can have Arrays of the Objects  
-   The function argument syntax is really powerful.  
-   Oftentimes people want to iterate through iterables or arrays.  
-   Oftentimes people want to check conditions.  
-   Python has list comprehensions.  
-   This is kind of like that, but simpler.  
-   You can have arguments as one argument, separated by “,,”  
-   make_server arg1,,arg2,,arg3,,arg4  
-   What's the point of using a scripting language when you can use C++?  
-   This uses FastCGI, so you can have an ____IDEAL____ webserver.  
-   You can have an IDEAL and very affordable website, that in a sense  
-   would be faster than Facebook.  
-   Facebook converts PHP to C++ (slow)  
-   This produces REAL C++, and it is very fast, almost as fast as  
-   possible.  
-   Native STL classes are used, like vector.  
-   Native STL classes are used, like vector and map  
-   Do you not need to run and child processes or do slow, costly things.  
-   You should want IDEAL.  
-   This is free software, and is BSD licensed.  
-   The function generation idea allows you to write in 1 line what other  
-   people might write in 50 lines.  
-   You do not need to compromise your ideals.  
-   You should want fast, efficient, and memory light programs that are not  
-   garbage collected (!!!) and that have reliable performance.  
-   C++, as everyone knows, delivers that.  
-   You should also want to not have to write a lot of code to do things.  
-   And you should also want safe, compiled code that checks things at  
-   compile time, so that bugs don't appear at run time.  
-   This program delivers.  
-   It uses NGINX ( a really, really common webserver) to help with the  
-   FastCGI.  
-   FastCGI, for the unfamiliar, is like normal CGI, but there aren't child  
-   processes.  
-   So the entire server could be written in idealistic C++ .  
-   Then you just have to think about scaling.  
-   There are some relevant links regarding scaling in the “scaling” file  
-   in the democracy project  
-   1) Speed  
-   2) Ease of writing code  
-   3) Memory usage  
-   4) Monetary costs  
-   5) Elegance  
-   6) Practicalness  
-   Those are 6 things.  
-   You don't have to sacrifice on those things.  
-   Contributions on this program would be really appreciated.  
-   It is called “make_server” for now.  
-   There was also a mode to generate javascript.  
-   I have to make that work again.  
-   The entire program is just one file.  
-   My email is gregorycohenvideos@gmail.com  
-   ### 10. Selectlines  
+   ### 7. Selectlines  
   
    selectlines shows all nonblank lines from the input  
    Example  
    cat file | selectlines  
    (echo 2; echo; echo; echo) | selectlines  
    => 2  
    The result would be 2, with no blank lines after that  
-   ### 11. Communicate  
-  
-   Communicate is cool.  
-   Communicate runs a Ruby expression after speaking a prompt (the first  
-   argument) and getting your verbal answer (using something unfortunately  
-   called "nerd-dictation", which is a wrapper around another program  
-   which deals with speech recognition)  
-   Communicate allows you to have conversations with your computer, and it  
-   is cross platform  
-   (Or it hopefully is)  
-   communicate 'What is the best color?' 'case text; when /blue/; puts  
-   "You are right!"; when /red/; puts "Red is a bad color"; end '  
-   That would be an example of how one could use "communicate"  
-   Make sure you have nerd-dictation on your computer  
-   The name nerd-dictation is absolutely awful, and I have to criticize  
-   him for not making it have a better name, but it works.  
-   ### 12. Executable  
-  
-   Makes all the files in the current directory executable  
-   ### 13. Processes  
+   ### 8. Processes  
   
    Processes lists all processes with a certain name  
    For example  
    processes sh  
    processes bash  
    processes ruby  
    processes gsub  
-   ### 14. Emeraldc  
+   ### 9. Emeraldc  
   
    The Ultimate C Preprocessor  
    I'm naming this preprocessor “Emerald C.”  
     Link  
    Howdy!  
    First, let me state that I am very much a perfectionist.  
    C is a wonderful language. C is probably the perfect programming  
@@ -461,88 +353,96 @@
    Why not use Rust?  
    $ time rustc a.rs  
    real 0m0.637s  
    user 0m0.502s  
    sys 0m0.160s  
    Rust takes 0.637 seconds to compile an empty file!  
    That is not ideal.  
-   ### 15. Last Nth  
+   ### 10. Last Nth  
   
    Last nth gets the last n lines from the standard input  
-   ### 16. Speakcat  
+   ### 11. Speakcat  
   
    Speak cat is a tool like “cat”, which shows the content of files  
    (technically, it combines the content of files).  
    But speak cat also speaks the text.  
    Which could be useful in some circumstances.  
    It's kind of like “tee” to your ear.  
-   ### 17. UCA CLI  
+   ### 12. UCA CLI  
   
    CLI for uca app  
-   ### 18. Big Num  
+   ### 13. Big Num  
   
    ![UCA](./images/10.png)  
-   ### 19. Squeeze  
+   ### 14. Squeeze  
   
    Squeeze reads all input from stdin, then it prints it back omitting  
    argument 1 line from the front, and argument 2 lines from the back  
    Example  
    squeeze 1 1  
    This would omit the first line and the last line  
    squeeze 5 3  
    This would omit the first 5 lines and the last 3 lines  
    squeeze 2 2 [file] also works, it outputs text to file  
-   ### 20. Foreach  
-  
-   Reads a bunch of lines  
-   Then a ruby expression is evaluated as the last line  
-   The result is outputted in an argument.  
-   You can enter /dev/null if you don't want an output file  
-   “t” is better  
-   See also  
-        t  
-   ### 21. Dictate  
+   ### 15. Dictate  
   
    Dictate opens web pages in emerald browser, or in any browser  
    (depending on the environment variable set), by you speaking, instead  
    of typing.  
    There is a mode called c_mode, that allows you to make code from  
    speaking.  
-   ### 22. Prepend  
+   ### 16. Prepend  
   
    prepend prepends input taken from the standard input to a file  
    Usage  
    prepend [file]  
    This is text to be prepended  
-   ### 23. Chat Rb  
+   ### 17. Chat Rb  
   
    This program is excellent.  
    It's essentially a mix of ChatGPT and a shell, such as bash or ZSH.  
    It has a bunch of features.  
    It can display a file or change to a folder just by mentioning it.  
    It outputs chatgpt data to an output folder in home folder and copies  
    it to clipboard  
    To run a shell command, prefix things with “c”, such as c gcc.....  
-   ### 24. Undump  
+   ### 18. Undump  
   
    undump is the opposite of dump  
    Example  
    echo cat | dump | undump  
    => cat  
    echo cat | dump  
    => “cat”  
    echo '“cat”' | undump  
    => cat  
-   ### 25. Append  
+   ### 19. Append  
   
    Appends text to file  
    Example  
    append file  
    This is more text to be appended  
-   ### 26. Rhyme  
+   ### 20. Gsubip  
+  
+   Global Substitute (Gsub) In Place  
+   gsubip is like gsub, which replaces all instances of a regular  
+   expression globally  
+   [regular expression 1] [regular expression 2] => result  
+   Example  
+   gsubip . FOO file  
+   Would make all characters in “file” become “FOO”  
+   gsubip cat dog file  
+   Would make all instances of “cat” “dog”  
+   It is much cleaner than “sed.”  
+   You don't need to have “sed” installed to run this program.  
+   It doesn't read from the standard input  
+   It takes exactly 3 arguments, no more, no fewer.  
+   See also  
+        gsub  
+   ### 21. Rhyme  
   
    A very powerful music generator program that doesn't use AI.  
     See this channel as an example of potential usage of this public  
    domain content  
    https://www.youtube.com/@LawrenceStevensMusic  
    The music industry is plagued with very foundational problems.  
    For starters, the quality of the discourse in music is very low, and  
@@ -715,46 +615,56 @@
    Their sucked in their circle, they never wave  
    Away from the truth, on the outskirt  
    With pre-thought of ideas, they automatically assert  
    Any progress is fleeting with them, they revert  
    Disingenuous to the extreme, the society they subvert  
    The society is the ones who hurt  
    ---  
-   ### 27. Email  
+   ### 22. Email  
   
    This currently doesn't work for gmail since 2022 due to policy changes.  
    A simple and practical tool to email people using Himalaya  
    Himalaya needs to be installed first  
    You would need to configure the script by changing its source code.  
    Modes  
    email [no arguments]  
    Email [yourself]  
    email [addr]  
    Email one email address  
    email [Subject] [addr] [option more addrs]  
    Example  
    email 'Gregory, I love your software!' gregorycohenvideos@gmail.com  
    my_friend@outlook.com person@example.com  
-   ### 28. Floor  
+   ### 23. Floor  
   
    Gets the floor of numbers e.g. 21.3 -> 21  
-   ### 29. Rgsub  
+   ### 24. Rgsub  
   
    Recursively replaces text.  
    Verbosely tells you everything that happens.  
    Non-regex.  
    Example  
    rgsub my_email@site.com my_second_email@site.com  
    Would replace an email recursively in a directory.  
-   It tries to skip non-text files.  
-   ### 30. Lines  
+   It tries to skip non-text files and hidden files.  
+   ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~  
+                Usage: rgsub   [optional list of files instead of recursive sear  
+ch]  
+                If a file is "-" or stdin, read from stdin and output to stdout.  
+                Options  
+                    -r, rename files instead of replacing contents of files.  
+                        find and replace in file and dir names instead  
+                    -v, verbose mode  
+                    -- Indicate end of options.  
+  
+   ### 25. Lines  
   
    Lines gets the number of files in the current folder that you are in.  
    It can also act like “wc -l” if you pipe data into it.  
-   ### 31. Clock  
+   ### 26. Clock  
   
    clock is useful  
    clock is a command line alarm clock  
    It wakes you up at 8:14, or at a time specified  
    Usage  
    clock  
    Runs clock  
@@ -763,22 +673,22 @@
    clock 9 0  
    Sets an alarm clock for 9 in the morning  
    It uses flite to wake you up  
    It speaks with a bunch of voices  
    To stop it  
    Run this command  
    clock stop  
-   ### 32. Emoji  
+   ### 27. Emoji  
   
    Emoji converts words to emojis from the standard input  
    It can also speak the output  
    It can also copy the output to your clipboard  
    It is very useful  
    ![UCA](./images/6.png)  
-   ### 33. Close  
+   ### 28. Close  
   
    “Close” is a simple program that closes “Emerald Browser,” a new web  
    browser based on the same engine as Chrome. Currently, Emerald Browser  
    only works on Linux and Mac (Or Windows with Windows Subsystem for  
    Linux or a Virtual Machine, but getting it to work might be tricky).  
    “close” closes the Web Browser, which is normally full-screen.  
    More accurately, it kills the browser, and all other copies of Emerald  
@@ -804,63 +714,71 @@
    Emerald browser has a built in the top. The terminal is the navigation  
    bar.  
    Some more work needs to be put into the browser.  
    Currently, new tabs can't be opened, which might be a dealbreaker for  
    some people.  
    Currently, content, like YouTube videos, can't be made fullscreen.  
    If anyone wants to contribute, feel free to!  
-   ### 34. Copy  
+   ### 29. Copy  
   
    copy copies the standard input  
    Example  
    ls | copy  
-   ### 35. Gsub  
+   ### 30. Gsub  
   
    Gsub is very powerful.  
    Usage  
    gsub [regular expression] [replacement text]  
    Example  
    cat text | gsub man dog  
    cat text | gsub 'man|boy|cat|dog' food  
    ls | gsub Desktop cat  
-   ### 36. News  
+   ### 31. News  
   
    Gets the news from bbc  
    Usage  
    news  
    news speak  
    uses google_speak to SPEAK the news, one story at a time.  
    ![UCA](./images/5.png)  
-   ### 37. Dump  
+   ### 32. Dump  
   
    Dump surrounds its input with quotes  
    ls | dump  
    => “....”  
    Use undump to get the reverse  
    See also  
         undump  
-   ### 38. Args  
+   ### 33. Args  
   
    args is like a better xargs  
    args works properly with spaces in the name of commands  
    It takes exactly one argument  
    Example  
    ls | args “mv -t ../f”  
-   ### 39. Quot  
+   ### 34. Rnip  
+  
+   Replace Not In Place  
+   This is like gsub, but for strings, not for regular expressions  
+   Example  
+   echo .......... | rnip foo bar  
+   See also  
+        gsub  
+   ### 35. Quot  
   
    Turns quotes in text into good text and makes text presentable.  
    Example  
    $ echo 'Joe said,        "One two three".' | quot  
    Joe said, “One two three.”  
    Example 2  
    quot < essay  
    Example 3  
    (Quote the file and output it)  
    quot text_file  
-   ### 40. Open  
+   ### 36. Open  
   
    “open” is a very efficient program that searches a query from google,  
    and then opens it in Emerald Browser.  
    If you ever want something to “just open”, you can use it.  
    Example  
    open “cats”  
    An earlier version of open worked like this  
@@ -873,65 +791,65 @@
    open “cats” “dogs” “frogs”  
    All of those queries would open in Emerald Browser.  
    Just make sure it is compiled in multipane mode if you want to open  
    multiple new sites at the same time.  
    See also  
         emerald-browser  
    close  
-   ### 41. Swap  
+   ### 37. Swap  
   
    Swaps two files  
    Example  
    swap text1 text2  
-   ### 42. Exp  
+   ### 38. Exp  
   
    exp is an exponentiation tool  
    (echo 5; echo 3) | exp  
    => 125  
    (echo 2; echo 10) | exp  
    => 1024  
-   ### 43. Div  
+   ### 39. Div  
   
    Divides numbers  
    Example  
    (echo 5000; echo 100) | div  
    => 50  
-   ### 44. Mul  
+   ### 40. Mul  
   
    Multiply numbers  
    echo 1 > file  
    echo 2 >> file  
    echo 3 >> file  
    echo 4 >> file  
    echo 5 >> file  
    cat file | mul  
    => 120  
-   ### 45. Nth  
+   ### 41. Nth  
   
    Nth gets the nth line from the input  
-   ### 46. Abs  
+   ### 42. Abs  
   
    Abs gets the absolute value of an integer  
    The absolute value of a number is the value of that number without its  
    sign  
    echo -300 | abs  
    => 300  
    echo 200 | abs  
    => 200  
    (echo -2; echo -10) | sub | abs  
    => 12  
    The last one would do -2 - -10, the result would be -12, and then the  
    absolute value would be computed, and so the result would be 12.  
-   ### 47. Add  
+   ### 43. Add  
   
    See the sub example  
    add adds integers from the standard input  
    (echo 1; echo 2; echo 3) | add  
    The result would be 6  
-   ### 48. Sub  
+   ### 44. Sub  
   
    Sub is a simple command line program that subtracts integers.  
    For some reason, no simple program did this.  
    Which is weird  
    Example  
    sub  
    (Input)  
@@ -940,23 +858,30 @@
    1  
    Result =>  
    6  
    Example  
    (echo 5; echo 2) | sub  
    Result =>  
    3  
-   ### 49. G+  
+   ### 45. Rip  
+  
+   Replace In Place  
+   rip tool replaces a string, not a regular expression, with another  
+   string  
+   Example  
+   rip cat dog file  
+   ### 46. G+  
   
    A compiler for C += 2. If you want to use C++ with Python syntax, you  
    can use this.  
    Usage is like g++  
    Example  
    g+ a.cpp -o out  
    See also README file & emerald-browser and its source  
-   ### 50. T  
+   ### 47. T  
   
    “t” is incredibly useful.  
    It can be used many, many times every day by computer power users.  
    It is kind of like “sed”, or perl, python or ruby.  
    It's the ULTIMATE shell “glue” tool.  
    t reads every line from the standard input, and for every line, it  
    evaluates a ruby expression  
@@ -980,67 +905,65 @@
    That processes every word in the dictionary, and says that every word  
    “is a good word.”  
    There are other programs in this software project like “t”.  
    But if you do command line text filtering, t might be the best tool  
    that you will find.  
    See also  
         gsub  
-   gsub_in_place  
+   gsubip  
+   .  
   
 Navigation  
   
     Top  
-    Ultimate Chat Application  
-    Discourse Generator  
-    Replace Not In Place  
-    Replace In Place  
+    Ultimate Chat Application.exe  
+    Discourse Generator.exe  
     Emerald Browser  
-    Gsub In Place  
+    Left Right.exe  
     Find Housing  
     Google Speak  
-    Make Server  
     Selectlines  
-    Communicate  
-    Executable  
     Processes  
     Emeraldc  
     Last Nth  
     Speakcat  
     Uca Cli  
     Big Num  
     Squeeze  
-    Foreach  
     Dictate  
     Prepend  
     Chat Rb  
     Undump  
     Append  
+    Gsubip  
     Rhyme  
     Email  
     Floor  
     Rgsub  
     Lines  
     Clock  
     Emoji  
     Close  
     Copy  
     Gsub  
     News  
     Dump  
     Args  
+    Rnip  
     Quot  
     Open  
     Swap  
     Exp  
     Div  
     Mul  
     Nth  
     Abs  
     Add  
     Sub  
+    Rip  
     G+  
     T  
   
 References  
   
    1. https://www.youtube.com/embed/Fx9x8cArK30  
    2. mailto:gregorycohenvideos@gmail.com
```

### Comparing `democracy-1.0.24/pyproject.toml` & `democracy-1.0.25/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "democracy"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.24"  # Required
+version = "1.0.25"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Trying to help with democracy, see https://github.com/gregoryc/democracy"  # Optional
 
 # This is an optional longer description of your project that represents
```

