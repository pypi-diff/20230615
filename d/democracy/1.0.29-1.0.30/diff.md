# Comparing `tmp/democracy-1.0.29.tar.gz` & `tmp/democracy-1.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "democracy-1.0.29.tar", last modified: Thu Jun 15 06:03:07 2023, max compression
+gzip compressed data, was "democracy-1.0.30.tar", last modified: Thu Jun 15 17:43:37 2023, max compression
```

## Comparing `democracy-1.0.29.tar` & `democracy-1.0.30.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 06:03:07.411506 democracy-1.0.29/
--rw-rw-r--   0 a         (1000) a         (1000)    39090 2023-06-15 06:03:07.411506 democracy-1.0.29/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)    38327 2023-06-15 06:02:45.000000 democracy-1.0.29/README.md
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 06:03:07.407506 democracy-1.0.29/democracy.egg-info/
--rw-rw-r--   0 a         (1000) a         (1000)    39090 2023-06-15 06:03:07.000000 democracy-1.0.29/democracy.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)      156 2023-06-15 06:03:07.000000 democracy-1.0.29/democracy.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-15 06:03:07.000000 democracy-1.0.29/democracy.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1000) a         (1000)        5 2023-06-15 06:03:07.000000 democracy-1.0.29/democracy.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)     5609 2023-06-15 06:02:03.000000 democracy-1.0.29/pyproject.toml
--rw-rw-r--   0 a         (1000) a         (1000)       38 2023-06-15 06:03:07.411506 democracy-1.0.29/setup.cfg
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 17:43:37.540201 democracy-1.0.30/
+-rw-rw-r--   0 a         (1000) a         (1000)    39039 2023-06-15 17:43:37.540201 democracy-1.0.30/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)    38276 2023-06-15 17:43:21.000000 democracy-1.0.30/README.md
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 17:43:37.540201 democracy-1.0.30/democracy.egg-info/
+-rw-rw-r--   0 a         (1000) a         (1000)    39039 2023-06-15 17:43:37.000000 democracy-1.0.30/democracy.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)      156 2023-06-15 17:43:37.000000 democracy-1.0.30/democracy.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-15 17:43:37.000000 democracy-1.0.30/democracy.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        5 2023-06-15 17:43:37.000000 democracy-1.0.30/democracy.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)     5609 2023-06-15 17:43:16.000000 democracy-1.0.30/pyproject.toml
+-rw-rw-r--   0 a         (1000) a         (1000)       38 2023-06-15 17:43:37.540201 democracy-1.0.30/setup.cfg
```

### Comparing `democracy-1.0.29/PKG-INFO` & `democracy-1.0.30/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,10 @@
-Metadata-Version: 2.1
-Name: democracy
-Version: 1.0.29
-Summary: Trying to help with democracy, see https://github.com/gregoryc/democracy
-Author-email: Gregory Cohen <gregorycohen2@gmail.com>
-Maintainer-email: Gregory Cohen <gregorycohen2@gmail.com>
-Project-URL: Homepage, https://github.com/gregoryc/democracy
-Keywords: ai,empowerment,agi,agis
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=2.0
-Description-Content-Type: text/markdown
-
 <h1 style='color: green'>Practical Self-Empowerment Utilities Covering Every Facet of Life </h1>
-      <iframe width="80%" height="600" src="https://www.youtube.com/embed/Fx9x8cArK30" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
+  
+  [![Video](https://img.youtube.com/vi/Fx9x8cArK30/maxresdefault.jpg)](https://www.youtube.com/watch?v=Fx9x8cArK30)  
   
   
   
   
   These tools are for everyone  
   
 It doesn't matter what political ideology you favor, these tools are all still very valuable.  
@@ -44,15 +27,15 @@
    There is also an idealistic make_server program that would make a very  
    fast webserver.  
    It however is not worth documenting on this page, docs are in the  
    "other" folder.  
    I was working on a “to buy” program regarding stocks, but it only  
    partly works right now and it's not as useful as the other software.  
    The find housing tool actually helped me to find housing in real life.  
-   Those aside, there are these 83 programs.  
+   Those aside, there are these 86 programs.  
    Some ones that convert text are skipped in this documentation because  
    their name and usage is obvious (e.g., color tools).  
   
 All of these programs are mostly self-contained. This is a really good thing.  
 You can use them anywhere without dependencies.  
   
    My email is  gregorycohenvideos@gmail.com and I really would like to  
@@ -110,15 +93,15 @@
   
    So I will leave a legacy. THIS MATERIAL WILL BE USED AND UNDERSTOOD.  
   
    And I will be found by AIs, assuming they continue to exist.  
   
     Democracy Github       Ruby Gem       Python PIP Package  
   
-Without further ado, here are the 83 documented programs. (The obvious usage  
+Without further ado, here are the 86 documented programs. (The obvious usage  
 ones are omitted.)  
   
    ### 1. Ultimate Chat Application.exe  
   
    ![UCA](./images/2.png)  
    There is so much potential with this program.  
    This is a non-AI chatbot. It's not based on generative AI or AI of any  
@@ -180,55 +163,61 @@
    ### 3. Emerald Browser  
   
    ![UCA](./images/3.png)  
    ![UCA](./images/4.png)  
    Emerald browser is a really powerful new browser  
    See README  
    It works based on panes.  
-   Read the documentation for “open”, “close” and also the README file.  
+   Read the documentation for “open,” “close” and also the README file.  
    ### 4. Left Right.exe  
   
    This is a tool to bring sanity to politics.  
    ![UCA](./images/12.png)  
    It gets viewpoints from the person that see the good in each political  
    side, left, right, left, right, etc.  
    It then presents all of that.  
    Hopefully this can make people more sane and less hyper-partisan.  
    ### 5. Find Housing  
   
    This is a nice tool to find housing with.  
    It is a nice, simple command line tool. You enter the minimum and  
    maximum prices, and Kijiji opens with your options.  
    This tool kind of actually helped me to find housing in real life.  
-   The default city is "Ottawa". You can easily change this.  
-   ### 6. Google Speak  
+   The default city is “Ottawa.” You can easily change this.  
+   ### 6. Prepend Each  
+  
+   Prepends a string to each line  
+   ### 7. Google Speak  
   
    Google speak is really useful. It speaks a statement using the Google  
    Translate voice, which is probably the most authoritative and  
    high-quality text-to-speech voice that exists.  
    It's kind of like “espeak” or similar tools, but it is much better.  
    You need an internet connection for it to work.  
    It is probably limited at 100 characters.  
-   ### 7. Selectlines  
+   ### 8. Append Each  
+  
+   Appends a string to each line  
+   ### 9. Selectlines  
   
    selectlines shows all nonblank lines from the input  
    Example  
    cat file | selectlines  
    (echo 2; echo; echo; echo) | selectlines  
    => 2  
    The result would be 2, with no blank lines after that  
-   ### 8. Processes  
+   ### 10. Processes  
   
    Processes lists all processes with a certain name  
    For example  
    processes sh  
    processes bash  
    processes ruby  
    processes gsub  
-   ### 9. Emeraldc  
+   ### 11. Emeraldc  
   
    The Ultimate C Preprocessor  
    I'm naming this preprocessor “Emerald C.”  
     Link  
    Howdy!  
    First, let me state that I am very much a perfectionist.  
    C is a wonderful language. C is probably the perfect programming  
@@ -251,29 +240,29 @@
    If one runs the command line preprocessor, with the “--features” flag,  
    the program shows all of its features  
    A Better C  
    C is a fantastic language. C compiles insanely fast, is the fastest  
    language there is, is very clear, is native to all systems, and is  
    useful for all purposes.  
    Some people, e.g., Bjarne Stroustrup, consider that C is “not good  
-   enough”, and make languages like C++ or D (or thousands of others)  
+   enough,” and make languages like C++ or D (or thousands of others)  
    This is not necessary.  
    There is no reason to use Python instead of C for “simple scripting  
    tasks”  
    Some functions can be used as methods  
    Makes for an excellent “scripting language” (which is really just  
    native C without things making it slow)  
    1 String Interpolation “String interplation like this #{foo} ” Calls  
    the join() function (talked about below to join strings,  
-   delim is a static global in each module called “sep”.  
+   delim is a static global in each module called “sep.”  
    Make sure you free() the string after. The string is stored in a static  
-   global variable called “last”.  
+   global variable called “last.”  
    So you could do puts(...); free(last)  
-   2 ew *i.ew “Foo”, a.ew “bar” | char* ends with another char*?  
-   3 sw *i.sw “Foo”, a.sw “bar” | char* starts with another char*?  
+   2 ew *i.ew “Foo,” a.ew “bar” | char* ends with another char*?  
+   3 sw *i.sw “Foo,” a.sw “bar” | char* starts with another char*?  
    4 == Comparison of strs, “foo” == “bar”  
    5 strip Returns pointer to string that was stripped, in place  
    6 chomp void function, chomps end of string of spaces, i.chomp or  
    chomp(i), in place  
    7 gsub Just like ruby, there is a gsub function.  
    The preprocessor detects if you use and adds -lpcre2-8 to the link  
    flags if you use it. Use $" for substitutions in argument 3 gsub(a, b,  
@@ -352,79 +341,81 @@
    Why not use Rust?  
    $ time rustc a.rs  
    real 0m0.637s  
    user 0m0.502s  
    sys 0m0.160s  
    Rust takes 0.637 seconds to compile an empty file!  
    That is not ideal.  
-   ### 10. Last Nth  
+   ### 12. Nth Word  
   
-   Last nth gets the last n lines from the standard input  
-   ### 11. Speakcat  
+   nth_word gets the nth word of each line  
+   For example  
+   nth_word 3  
+   gets the 3rd word of each line  
+   ### 13. Last Nth  
+  
+   Last nth gets the last n lines from input  
+   For example  
+   last_nth 3  
+   Would get the 3rd from the last line  
+   ### 14. Speakcat  
   
-   Speak cat is a tool like “cat”, which shows the content of files  
+   Speak cat is a tool like “cat,” which shows the content of files  
    (technically, it combines the content of files).  
    But speak cat also speaks the text.  
    Which could be useful in some circumstances.  
    It's kind of like “tee” to your ear.  
-   ### 12. UCA CLI  
+   ### 15. UCA CLI  
   
    CLI for uca app  
-   ### 13. Big Num  
+   ### 16. Big Num  
   
    ![UCA](./images/10.png)  
-   ### 14. Squeeze  
+   ### 17. Squeeze  
   
    Squeeze reads all input from stdin, then it prints it back omitting  
    argument 1 line from the front, and argument 2 lines from the back  
    Example  
    squeeze 1 1  
    This would omit the first line and the last line  
    squeeze 5 3  
    This would omit the first 5 lines and the last 3 lines  
    squeeze 2 2 [file] also works, it outputs text to file  
-   ### 15. Dictate  
+   ### 18. Dictate  
   
    Dictate opens web pages in emerald browser, or in any browser  
    (depending on the environment variable set), by you speaking, instead  
    of typing.  
    There is a mode called c_mode, that allows you to make code from  
    speaking.  
-   ### 16. Prepend  
+   ### 19. Prepend  
   
    prepend prepends input taken from the standard input to a file  
    Usage  
    prepend [file]  
    This is text to be prepended  
-   ### 17. Chat Rb  
+   ### 20. Chat Rb  
   
    This program is excellent.  
    It's essentially a mix of ChatGPT and a shell, such as bash or ZSH.  
    It has a bunch of features.  
    It can display a file or change to a folder just by mentioning it.  
    It outputs chatgpt data to an output folder in home folder and copies  
    it to clipboard  
-   To run a shell command, prefix things with “c”, such as c gcc.....  
-   ### 18. Undump  
-  
-   undump is the opposite of dump  
-   Example  
-   echo cat | dump | undump  
-   => cat  
-   echo cat | dump  
-   => “cat”  
-   echo '“cat”' | undump  
-   => cat  
-   ### 19. Append  
+   To run a shell command, prefix things with “c,” such as c gcc.....  
+   ### 21. Append  
   
    Appends text to file  
    Example  
    append file  
    This is more text to be appended  
-   ### 20. Gsubip  
+   ### 22. Delete  
+  
+   Recursively delete all files named a certain name.  
+   ### 23. Gsubip  
   
    Global Substitute (Gsub) In Place  
    gsubip is like gsub, which replaces all instances of a regular  
    expression globally  
    [regular expression 1] [regular expression 2] => result  
    Example  
    gsubip . FOO file  
@@ -433,15 +424,15 @@
    Would make all instances of “cat” “dog”  
    It is much cleaner than “sed.”  
    You don't need to have “sed” installed to run this program.  
    It doesn't read from the standard input  
    It takes exactly 3 arguments, no more, no fewer.  
    See also  
         gsub  
-   ### 21. Rhyme  
+   ### 24. Rhyme  
   
    A very powerful music generator program that doesn't use AI.  
     See this channel as an example of potential usage of this public  
    domain content  
    https://www.youtube.com/@LawrenceStevensMusic  
    The music industry is plagued with very foundational problems.  
    For starters, the quality of the discourse in music is very low, and  
@@ -449,15 +440,15 @@
    as during the era in which classical music was popular and before.  
    People aren't able to fight back, against superficiality and potential  
    deception in messages.  
    One of the greatest problems in the current world is the mainstream  
    scientific establishment, supported and upheld by mainstream academia.  
    To indicate what is already obvious, it exists in the context of a  
    legacy of authoritarianism and a lack of understanding of dynamism.  
-   It is not dynamic or forceful, the "results" of it don't change the  
+   It is not dynamic or forceful, the “results” of it don't change the  
    foundation of society. True free discourse is not supported, especially  
    in regards to the human mind and human well-being and human freedom.  
    These problems should be opposed and fought, it is self-evident that  
    this would be the best use of ones time, for it would lead to true  
    freedom.  
    One excellent way to combat this would be to use the generated songs  
    generated by a computer program called Rhyme, available at  
@@ -476,15 +467,15 @@
    Shoving art and flippant content in ones face, is the best way of doing  
    such.  
    Accountability must always be brought about.  
    Is music good and desired? For sure.  
    USAGE OF PROGRAM  
    Enter basename to make songs folder in (folder/songs, num songs =  
    13000)  
-   Usage rhyme [folder] (processes files "1.json" and "21.json" by  
+   Usage rhyme [folder] (processes files “1.json” and “21.json” by  
    default)  
    Example output of a song  
    ![UCA](./images/7.png)  
    (NO COPYRIGHT RESTRICTIONS ON THIS CONTENT WHATSOEVER. FULLY PUBLIC  
    DOMAIN)  
    Name the song or poem as you wish, resell it, but please positively  
    influence culture  
@@ -577,15 +568,15 @@
    Working don't matter for this, whether day or graveyard  
    They don't care about your feelings, they don't regard  
    They are failures, down at the boulevard  
    They don't have decency, they automatically disregard  
    They're a complete failure, they only neglect  
    They don't speak the language of the people or their dialect  
    This is not right, this is completely incorrect  
-   The only focus on “responses”, they just want to deflect  
+   The only focus on “responses,” they just want to deflect  
    The lies are put forth, the lies they erect  
    CHORUS  
    They're such failures, themselves they outdid  
    Cutting out the conversation, putting on the lid  
    Don't have to do with ego or id  
    Running away from conversation just like a kid  
    Their neglect is out of this world, I swear it's avant-garde  
@@ -614,56 +605,55 @@
    Their sucked in their circle, they never wave  
    Away from the truth, on the outskirt  
    With pre-thought of ideas, they automatically assert  
    Any progress is fleeting with them, they revert  
    Disingenuous to the extreme, the society they subvert  
    The society is the ones who hurt  
    ---  
-   ### 22. Email  
+   ### 25. Email  
   
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
-   ### 23. Floor  
+   ### 26. Floor  
   
    Gets the floor of numbers e.g. 21.3 -> 21  
-   ### 24. Rgsub  
+   ### 27. Rgsub  
   
    Recursively replaces text.  
    Verbosely tells you everything that happens.  
    Non-regex.  
    Example  
    rgsub my_email@site.com my_second_email@site.com  
    Would replace an email recursively in a directory.  
    It tries to skip non-text files and hidden files.  
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~  
-                Usage: rgsub   [optional list of files instead of recursive sear  
-ch]  
-                If a file is "-" or stdin, read from stdin and output to stdout.  
-                Options  
-                    -r, rename files instead of replacing contents of files.  
-                        find and replace in file and dir names instead  
-                    -v, verbose mode  
-                    -- Indicate end of options.  
+        Usage: rgsub   [optional list of files instead of recursive search]  
+        If a file is “-” or stdin, read from stdin and output to stdout.  
+        Options  
+        -r, rename files instead of replacing contents of files.  
+        find and replace in file and dir names instead  
+        -v, verbose mode  
+        -- Indicate end of options.  
   
-   ### 25. Lines  
+   ### 28. Lines  
   
    Lines gets the number of files in the current folder that you are in.  
    It can also act like “wc -l” if you pipe data into it.  
-   ### 26. Clock  
+   ### 29. Clock  
   
    clock is useful  
    clock is a command line alarm clock  
    It wakes you up at 8:14, or at a time specified  
    Usage  
    clock  
    Runs clock  
@@ -672,22 +662,22 @@
    clock 9 0  
    Sets an alarm clock for 9 in the morning  
    It uses flite to wake you up  
    It speaks with a bunch of voices  
    To stop it  
    Run this command  
    clock stop  
-   ### 27. Emoji  
+   ### 30. Emoji  
   
    Emoji converts words to emojis from the standard input  
    It can also speak the output  
    It can also copy the output to your clipboard  
    It is very useful  
    ![UCA](./images/6.png)  
-   ### 28. Close  
+   ### 31. Close  
   
    “Close” is a simple program that closes “Emerald Browser,” a new web  
    browser based on the same engine as Chrome. Currently, Emerald Browser  
    only works on Linux and Mac (Or Windows with Windows Subsystem for  
    Linux or a Virtual Machine, but getting it to work might be tricky).  
    “close” closes the Web Browser, which is normally full-screen.  
    More accurately, it kills the browser, and all other copies of Emerald  
@@ -713,75 +703,70 @@
    Emerald browser has a built in the top. The terminal is the navigation  
    bar.  
    Some more work needs to be put into the browser.  
    Currently, new tabs can't be opened, which might be a dealbreaker for  
    some people.  
    Currently, content, like YouTube videos, can't be made fullscreen.  
    If anyone wants to contribute, feel free to!  
-   ### 29. Copy  
+   ### 32. Copy  
   
    copy copies the standard input  
    Example  
    ls | copy  
-   ### 30. Gsub  
+   ### 33. Gsub  
   
    Gsub is very powerful.  
    Usage  
    gsub [regular expression] [replacement text]  
    Example  
    cat text | gsub man dog  
    cat text | gsub 'man|boy|cat|dog' food  
    ls | gsub Desktop cat  
-   ### 31. News  
+   ### 34. News  
   
    Gets the news from bbc  
    Usage  
    news  
    news speak  
    uses google_speak to SPEAK the news, one story at a time.  
    ![UCA](./images/5.png)  
-   ### 32. Dump  
-  
-   Dump surrounds its input with quotes  
-   ls | dump  
-   => “....”  
-   Use undump to get the reverse  
-   See also  
-        undump  
-   ### 33. Args  
+   ### 35. Args  
   
    args is like a better xargs  
    args works properly with spaces in the name of commands  
    It takes exactly one argument  
    Example  
    ls | args “mv -t ../f”  
-   ### 34. Rnip  
+   ### 36. Rnip  
   
    Replace Not In Place  
    This is like gsub, but for strings, not for regular expressions  
    Example  
    echo .......... | rnip foo bar  
    See also  
         gsub  
-   ### 35. Quot  
+   ### 37. Trim  
+  
+   Trims spaces of each line  
+   ### 38. Quot  
   
    Turns quotes in text into good text and makes text presentable.  
    Example  
    $ echo 'Joe said,        "One two three".' | quot  
    Joe said, “One two three.”  
    Example 2  
    quot < essay  
    Example 3  
    (Quote the file and output it)  
    quot text_file  
-   ### 36. Open  
+   ### 39. Open  
   
    “open” is a very efficient program that searches a query from google,  
    and then opens it in Emerald Browser.  
-   If you ever want something to “just open”, you can use it.  
+   If you ever want something to “just open,” you can use it.  
    Example  
    open “cats”  
    An earlier version of open worked like this  
    open [site1] [site2] [site3] N  
    site1, site2, and site3 would all be opened, and the top N queries were  
    all shown in different panes  
    An even earlier version of this program used Chrome to open the sites.  
@@ -790,65 +775,65 @@
    open “cats” “dogs” “frogs”  
    All of those queries would open in Emerald Browser.  
    Just make sure it is compiled in multipane mode if you want to open  
    multiple new sites at the same time.  
    See also  
         emerald-browser  
    close  
-   ### 37. Swap  
+   ### 40. Swap  
   
    Swaps two files  
    Example  
    swap text1 text2  
-   ### 38. Exp  
+   ### 41. Exp  
   
    exp is an exponentiation tool  
    (echo 5; echo 3) | exp  
    => 125  
    (echo 2; echo 10) | exp  
    => 1024  
-   ### 39. Div  
+   ### 42. Div  
   
    Divides numbers  
    Example  
    (echo 5000; echo 100) | div  
    => 50  
-   ### 40. Mul  
+   ### 43. Mul  
   
    Multiply numbers  
    echo 1 > file  
    echo 2 >> file  
    echo 3 >> file  
    echo 4 >> file  
    echo 5 >> file  
    cat file | mul  
    => 120  
-   ### 41. Nth  
+   ### 44. Nth  
   
    Nth gets the nth line from the input  
-   ### 42. Abs  
+   ### 45. Abs  
   
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
-   ### 43. Add  
+   ### 46. Add  
   
    See the sub example  
    add adds integers from the standard input  
    (echo 1; echo 2; echo 3) | add  
    The result would be 6  
-   ### 44. Sub  
+   ### 47. Sub  
   
    Sub is a simple command line program that subtracts integers.  
    For some reason, no simple program did this.  
    Which is weird  
    Example  
    sub  
    (Input)  
@@ -857,34 +842,34 @@
    1  
    Result =>  
    6  
    Example  
    (echo 5; echo 2) | sub  
    Result =>  
    3  
-   ### 45. Rip  
+   ### 48. Rip  
   
    Replace In Place  
    rip tool replaces a string, not a regular expression, with another  
    string  
    Example  
    rip cat dog file  
-   ### 46. G+  
+   ### 49. G+  
   
    A compiler for C += 2. If you want to use C++ with Python syntax, you  
    can use this.  
    Usage is like g++  
    Example  
    g+ a.cpp -o out  
    See also README file & emerald-browser and its source  
-   ### 47. T  
+   ### 50. T  
   
    “t” is incredibly useful.  
    It can be used many, many times every day by computer power users.  
-   It is kind of like “sed”, or perl, python or ruby.  
+   It is kind of like “sed,” or perl, python or ruby.  
    It's the ULTIMATE shell “glue” tool.  
    t reads every line from the standard input, and for every line, it  
    evaluates a ruby expression  
    t a + 2  
    would add 2 to every line  
    Number automatically get converted to numbers in Ruby.  
    So one doesn't have to worry about that.  
@@ -899,15 +884,15 @@
    echo “One line” | t a while true  
    The second line, again is a Ruby expression.  
    You can have really complex expressions on the second line.  
    You can even import modules.  
    cat /usr/share/dict/words | t 'a + “ is a good word.”'  
    That processes every word in the dictionary, and says that every word  
    “is a good word.”  
-   There are other programs in this software project like “t”.  
+   There are other programs in this software project like “t.”  
    But if you do command line text filtering, t might be the best tool  
    that you will find.  
    See also  
         gsub  
    gsubip  
    .  
   
@@ -915,43 +900,46 @@
   
     Top  
     Ultimate Chat Application.exe  
     Discourse Generator.exe  
     Emerald Browser  
     Left Right.exe  
     Find Housing  
+    Prepend Each  
     Google Speak  
+    Append Each  
     Selectlines  
     Processes  
     Emeraldc  
+    Nth Word  
     Last Nth  
     Speakcat  
     Uca Cli  
     Big Num  
     Squeeze  
     Dictate  
     Prepend  
     Chat Rb  
-    Undump  
     Append  
+    Delete  
     Gsubip  
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
-    Dump  
     Args  
     Rnip  
+    Trim  
     Quot  
     Open  
     Swap  
     Exp  
     Div  
     Mul  
     Nth
```

### Comparing `democracy-1.0.29/README.md` & `democracy-1.0.30/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,28 @@
+Metadata-Version: 2.1
+Name: democracy
+Version: 1.0.30
+Summary: Trying to help with democracy, see https://github.com/gregoryc/democracy
+Author-email: Gregory Cohen <gregorycohen2@gmail.com>
+Maintainer-email: Gregory Cohen <gregorycohen2@gmail.com>
+Project-URL: Homepage, https://github.com/gregoryc/democracy
+Keywords: ai,empowerment,agi,agis
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=2.0
+Description-Content-Type: text/markdown
+
 <h1 style='color: green'>Practical Self-Empowerment Utilities Covering Every Facet of Life </h1>
-      <iframe width="80%" height="600" src="https://www.youtube.com/embed/Fx9x8cArK30" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
+  
+  [![Video](https://img.youtube.com/vi/Fx9x8cArK30/maxresdefault.jpg)](https://www.youtube.com/watch?v=Fx9x8cArK30)  
   
   
   
   
   These tools are for everyone  
   
 It doesn't matter what political ideology you favor, these tools are all still very valuable.  
@@ -26,15 +45,15 @@
    There is also an idealistic make_server program that would make a very  
    fast webserver.  
    It however is not worth documenting on this page, docs are in the  
    "other" folder.  
    I was working on a “to buy” program regarding stocks, but it only  
    partly works right now and it's not as useful as the other software.  
    The find housing tool actually helped me to find housing in real life.  
-   Those aside, there are these 83 programs.  
+   Those aside, there are these 86 programs.  
    Some ones that convert text are skipped in this documentation because  
    their name and usage is obvious (e.g., color tools).  
   
 All of these programs are mostly self-contained. This is a really good thing.  
 You can use them anywhere without dependencies.  
   
    My email is  gregorycohenvideos@gmail.com and I really would like to  
@@ -92,15 +111,15 @@
   
    So I will leave a legacy. THIS MATERIAL WILL BE USED AND UNDERSTOOD.  
   
    And I will be found by AIs, assuming they continue to exist.  
   
     Democracy Github       Ruby Gem       Python PIP Package  
   
-Without further ado, here are the 83 documented programs. (The obvious usage  
+Without further ado, here are the 86 documented programs. (The obvious usage  
 ones are omitted.)  
   
    ### 1. Ultimate Chat Application.exe  
   
    ![UCA](./images/2.png)  
    There is so much potential with this program.  
    This is a non-AI chatbot. It's not based on generative AI or AI of any  
@@ -162,55 +181,61 @@
    ### 3. Emerald Browser  
   
    ![UCA](./images/3.png)  
    ![UCA](./images/4.png)  
    Emerald browser is a really powerful new browser  
    See README  
    It works based on panes.  
-   Read the documentation for “open”, “close” and also the README file.  
+   Read the documentation for “open,” “close” and also the README file.  
    ### 4. Left Right.exe  
   
    This is a tool to bring sanity to politics.  
    ![UCA](./images/12.png)  
    It gets viewpoints from the person that see the good in each political  
    side, left, right, left, right, etc.  
    It then presents all of that.  
    Hopefully this can make people more sane and less hyper-partisan.  
    ### 5. Find Housing  
   
    This is a nice tool to find housing with.  
    It is a nice, simple command line tool. You enter the minimum and  
    maximum prices, and Kijiji opens with your options.  
    This tool kind of actually helped me to find housing in real life.  
-   The default city is "Ottawa". You can easily change this.  
-   ### 6. Google Speak  
+   The default city is “Ottawa.” You can easily change this.  
+   ### 6. Prepend Each  
+  
+   Prepends a string to each line  
+   ### 7. Google Speak  
   
    Google speak is really useful. It speaks a statement using the Google  
    Translate voice, which is probably the most authoritative and  
    high-quality text-to-speech voice that exists.  
    It's kind of like “espeak” or similar tools, but it is much better.  
    You need an internet connection for it to work.  
    It is probably limited at 100 characters.  
-   ### 7. Selectlines  
+   ### 8. Append Each  
+  
+   Appends a string to each line  
+   ### 9. Selectlines  
   
    selectlines shows all nonblank lines from the input  
    Example  
    cat file | selectlines  
    (echo 2; echo; echo; echo) | selectlines  
    => 2  
    The result would be 2, with no blank lines after that  
-   ### 8. Processes  
+   ### 10. Processes  
   
    Processes lists all processes with a certain name  
    For example  
    processes sh  
    processes bash  
    processes ruby  
    processes gsub  
-   ### 9. Emeraldc  
+   ### 11. Emeraldc  
   
    The Ultimate C Preprocessor  
    I'm naming this preprocessor “Emerald C.”  
     Link  
    Howdy!  
    First, let me state that I am very much a perfectionist.  
    C is a wonderful language. C is probably the perfect programming  
@@ -233,29 +258,29 @@
    If one runs the command line preprocessor, with the “--features” flag,  
    the program shows all of its features  
    A Better C  
    C is a fantastic language. C compiles insanely fast, is the fastest  
    language there is, is very clear, is native to all systems, and is  
    useful for all purposes.  
    Some people, e.g., Bjarne Stroustrup, consider that C is “not good  
-   enough”, and make languages like C++ or D (or thousands of others)  
+   enough,” and make languages like C++ or D (or thousands of others)  
    This is not necessary.  
    There is no reason to use Python instead of C for “simple scripting  
    tasks”  
    Some functions can be used as methods  
    Makes for an excellent “scripting language” (which is really just  
    native C without things making it slow)  
    1 String Interpolation “String interplation like this #{foo} ” Calls  
    the join() function (talked about below to join strings,  
-   delim is a static global in each module called “sep”.  
+   delim is a static global in each module called “sep.”  
    Make sure you free() the string after. The string is stored in a static  
-   global variable called “last”.  
+   global variable called “last.”  
    So you could do puts(...); free(last)  
-   2 ew *i.ew “Foo”, a.ew “bar” | char* ends with another char*?  
-   3 sw *i.sw “Foo”, a.sw “bar” | char* starts with another char*?  
+   2 ew *i.ew “Foo,” a.ew “bar” | char* ends with another char*?  
+   3 sw *i.sw “Foo,” a.sw “bar” | char* starts with another char*?  
    4 == Comparison of strs, “foo” == “bar”  
    5 strip Returns pointer to string that was stripped, in place  
    6 chomp void function, chomps end of string of spaces, i.chomp or  
    chomp(i), in place  
    7 gsub Just like ruby, there is a gsub function.  
    The preprocessor detects if you use and adds -lpcre2-8 to the link  
    flags if you use it. Use $" for substitutions in argument 3 gsub(a, b,  
@@ -334,79 +359,81 @@
    Why not use Rust?  
    $ time rustc a.rs  
    real 0m0.637s  
    user 0m0.502s  
    sys 0m0.160s  
    Rust takes 0.637 seconds to compile an empty file!  
    That is not ideal.  
-   ### 10. Last Nth  
+   ### 12. Nth Word  
   
-   Last nth gets the last n lines from the standard input  
-   ### 11. Speakcat  
+   nth_word gets the nth word of each line  
+   For example  
+   nth_word 3  
+   gets the 3rd word of each line  
+   ### 13. Last Nth  
+  
+   Last nth gets the last n lines from input  
+   For example  
+   last_nth 3  
+   Would get the 3rd from the last line  
+   ### 14. Speakcat  
   
-   Speak cat is a tool like “cat”, which shows the content of files  
+   Speak cat is a tool like “cat,” which shows the content of files  
    (technically, it combines the content of files).  
    But speak cat also speaks the text.  
    Which could be useful in some circumstances.  
    It's kind of like “tee” to your ear.  
-   ### 12. UCA CLI  
+   ### 15. UCA CLI  
   
    CLI for uca app  
-   ### 13. Big Num  
+   ### 16. Big Num  
   
    ![UCA](./images/10.png)  
-   ### 14. Squeeze  
+   ### 17. Squeeze  
   
    Squeeze reads all input from stdin, then it prints it back omitting  
    argument 1 line from the front, and argument 2 lines from the back  
    Example  
    squeeze 1 1  
    This would omit the first line and the last line  
    squeeze 5 3  
    This would omit the first 5 lines and the last 3 lines  
    squeeze 2 2 [file] also works, it outputs text to file  
-   ### 15. Dictate  
+   ### 18. Dictate  
   
    Dictate opens web pages in emerald browser, or in any browser  
    (depending on the environment variable set), by you speaking, instead  
    of typing.  
    There is a mode called c_mode, that allows you to make code from  
    speaking.  
-   ### 16. Prepend  
+   ### 19. Prepend  
   
    prepend prepends input taken from the standard input to a file  
    Usage  
    prepend [file]  
    This is text to be prepended  
-   ### 17. Chat Rb  
+   ### 20. Chat Rb  
   
    This program is excellent.  
    It's essentially a mix of ChatGPT and a shell, such as bash or ZSH.  
    It has a bunch of features.  
    It can display a file or change to a folder just by mentioning it.  
    It outputs chatgpt data to an output folder in home folder and copies  
    it to clipboard  
-   To run a shell command, prefix things with “c”, such as c gcc.....  
-   ### 18. Undump  
-  
-   undump is the opposite of dump  
-   Example  
-   echo cat | dump | undump  
-   => cat  
-   echo cat | dump  
-   => “cat”  
-   echo '“cat”' | undump  
-   => cat  
-   ### 19. Append  
+   To run a shell command, prefix things with “c,” such as c gcc.....  
+   ### 21. Append  
   
    Appends text to file  
    Example  
    append file  
    This is more text to be appended  
-   ### 20. Gsubip  
+   ### 22. Delete  
+  
+   Recursively delete all files named a certain name.  
+   ### 23. Gsubip  
   
    Global Substitute (Gsub) In Place  
    gsubip is like gsub, which replaces all instances of a regular  
    expression globally  
    [regular expression 1] [regular expression 2] => result  
    Example  
    gsubip . FOO file  
@@ -415,15 +442,15 @@
    Would make all instances of “cat” “dog”  
    It is much cleaner than “sed.”  
    You don't need to have “sed” installed to run this program.  
    It doesn't read from the standard input  
    It takes exactly 3 arguments, no more, no fewer.  
    See also  
         gsub  
-   ### 21. Rhyme  
+   ### 24. Rhyme  
   
    A very powerful music generator program that doesn't use AI.  
     See this channel as an example of potential usage of this public  
    domain content  
    https://www.youtube.com/@LawrenceStevensMusic  
    The music industry is plagued with very foundational problems.  
    For starters, the quality of the discourse in music is very low, and  
@@ -431,15 +458,15 @@
    as during the era in which classical music was popular and before.  
    People aren't able to fight back, against superficiality and potential  
    deception in messages.  
    One of the greatest problems in the current world is the mainstream  
    scientific establishment, supported and upheld by mainstream academia.  
    To indicate what is already obvious, it exists in the context of a  
    legacy of authoritarianism and a lack of understanding of dynamism.  
-   It is not dynamic or forceful, the "results" of it don't change the  
+   It is not dynamic or forceful, the “results” of it don't change the  
    foundation of society. True free discourse is not supported, especially  
    in regards to the human mind and human well-being and human freedom.  
    These problems should be opposed and fought, it is self-evident that  
    this would be the best use of ones time, for it would lead to true  
    freedom.  
    One excellent way to combat this would be to use the generated songs  
    generated by a computer program called Rhyme, available at  
@@ -458,15 +485,15 @@
    Shoving art and flippant content in ones face, is the best way of doing  
    such.  
    Accountability must always be brought about.  
    Is music good and desired? For sure.  
    USAGE OF PROGRAM  
    Enter basename to make songs folder in (folder/songs, num songs =  
    13000)  
-   Usage rhyme [folder] (processes files "1.json" and "21.json" by  
+   Usage rhyme [folder] (processes files “1.json” and “21.json” by  
    default)  
    Example output of a song  
    ![UCA](./images/7.png)  
    (NO COPYRIGHT RESTRICTIONS ON THIS CONTENT WHATSOEVER. FULLY PUBLIC  
    DOMAIN)  
    Name the song or poem as you wish, resell it, but please positively  
    influence culture  
@@ -559,15 +586,15 @@
    Working don't matter for this, whether day or graveyard  
    They don't care about your feelings, they don't regard  
    They are failures, down at the boulevard  
    They don't have decency, they automatically disregard  
    They're a complete failure, they only neglect  
    They don't speak the language of the people or their dialect  
    This is not right, this is completely incorrect  
-   The only focus on “responses”, they just want to deflect  
+   The only focus on “responses,” they just want to deflect  
    The lies are put forth, the lies they erect  
    CHORUS  
    They're such failures, themselves they outdid  
    Cutting out the conversation, putting on the lid  
    Don't have to do with ego or id  
    Running away from conversation just like a kid  
    Their neglect is out of this world, I swear it's avant-garde  
@@ -596,56 +623,55 @@
    Their sucked in their circle, they never wave  
    Away from the truth, on the outskirt  
    With pre-thought of ideas, they automatically assert  
    Any progress is fleeting with them, they revert  
    Disingenuous to the extreme, the society they subvert  
    The society is the ones who hurt  
    ---  
-   ### 22. Email  
+   ### 25. Email  
   
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
-   ### 23. Floor  
+   ### 26. Floor  
   
    Gets the floor of numbers e.g. 21.3 -> 21  
-   ### 24. Rgsub  
+   ### 27. Rgsub  
   
    Recursively replaces text.  
    Verbosely tells you everything that happens.  
    Non-regex.  
    Example  
    rgsub my_email@site.com my_second_email@site.com  
    Would replace an email recursively in a directory.  
    It tries to skip non-text files and hidden files.  
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~  
-                Usage: rgsub   [optional list of files instead of recursive sear  
-ch]  
-                If a file is "-" or stdin, read from stdin and output to stdout.  
-                Options  
-                    -r, rename files instead of replacing contents of files.  
-                        find and replace in file and dir names instead  
-                    -v, verbose mode  
-                    -- Indicate end of options.  
+        Usage: rgsub   [optional list of files instead of recursive search]  
+        If a file is “-” or stdin, read from stdin and output to stdout.  
+        Options  
+        -r, rename files instead of replacing contents of files.  
+        find and replace in file and dir names instead  
+        -v, verbose mode  
+        -- Indicate end of options.  
   
-   ### 25. Lines  
+   ### 28. Lines  
   
    Lines gets the number of files in the current folder that you are in.  
    It can also act like “wc -l” if you pipe data into it.  
-   ### 26. Clock  
+   ### 29. Clock  
   
    clock is useful  
    clock is a command line alarm clock  
    It wakes you up at 8:14, or at a time specified  
    Usage  
    clock  
    Runs clock  
@@ -654,22 +680,22 @@
    clock 9 0  
    Sets an alarm clock for 9 in the morning  
    It uses flite to wake you up  
    It speaks with a bunch of voices  
    To stop it  
    Run this command  
    clock stop  
-   ### 27. Emoji  
+   ### 30. Emoji  
   
    Emoji converts words to emojis from the standard input  
    It can also speak the output  
    It can also copy the output to your clipboard  
    It is very useful  
    ![UCA](./images/6.png)  
-   ### 28. Close  
+   ### 31. Close  
   
    “Close” is a simple program that closes “Emerald Browser,” a new web  
    browser based on the same engine as Chrome. Currently, Emerald Browser  
    only works on Linux and Mac (Or Windows with Windows Subsystem for  
    Linux or a Virtual Machine, but getting it to work might be tricky).  
    “close” closes the Web Browser, which is normally full-screen.  
    More accurately, it kills the browser, and all other copies of Emerald  
@@ -695,75 +721,70 @@
    Emerald browser has a built in the top. The terminal is the navigation  
    bar.  
    Some more work needs to be put into the browser.  
    Currently, new tabs can't be opened, which might be a dealbreaker for  
    some people.  
    Currently, content, like YouTube videos, can't be made fullscreen.  
    If anyone wants to contribute, feel free to!  
-   ### 29. Copy  
+   ### 32. Copy  
   
    copy copies the standard input  
    Example  
    ls | copy  
-   ### 30. Gsub  
+   ### 33. Gsub  
   
    Gsub is very powerful.  
    Usage  
    gsub [regular expression] [replacement text]  
    Example  
    cat text | gsub man dog  
    cat text | gsub 'man|boy|cat|dog' food  
    ls | gsub Desktop cat  
-   ### 31. News  
+   ### 34. News  
   
    Gets the news from bbc  
    Usage  
    news  
    news speak  
    uses google_speak to SPEAK the news, one story at a time.  
    ![UCA](./images/5.png)  
-   ### 32. Dump  
-  
-   Dump surrounds its input with quotes  
-   ls | dump  
-   => “....”  
-   Use undump to get the reverse  
-   See also  
-        undump  
-   ### 33. Args  
+   ### 35. Args  
   
    args is like a better xargs  
    args works properly with spaces in the name of commands  
    It takes exactly one argument  
    Example  
    ls | args “mv -t ../f”  
-   ### 34. Rnip  
+   ### 36. Rnip  
   
    Replace Not In Place  
    This is like gsub, but for strings, not for regular expressions  
    Example  
    echo .......... | rnip foo bar  
    See also  
         gsub  
-   ### 35. Quot  
+   ### 37. Trim  
+  
+   Trims spaces of each line  
+   ### 38. Quot  
   
    Turns quotes in text into good text and makes text presentable.  
    Example  
    $ echo 'Joe said,        "One two three".' | quot  
    Joe said, “One two three.”  
    Example 2  
    quot < essay  
    Example 3  
    (Quote the file and output it)  
    quot text_file  
-   ### 36. Open  
+   ### 39. Open  
   
    “open” is a very efficient program that searches a query from google,  
    and then opens it in Emerald Browser.  
-   If you ever want something to “just open”, you can use it.  
+   If you ever want something to “just open,” you can use it.  
    Example  
    open “cats”  
    An earlier version of open worked like this  
    open [site1] [site2] [site3] N  
    site1, site2, and site3 would all be opened, and the top N queries were  
    all shown in different panes  
    An even earlier version of this program used Chrome to open the sites.  
@@ -772,65 +793,65 @@
    open “cats” “dogs” “frogs”  
    All of those queries would open in Emerald Browser.  
    Just make sure it is compiled in multipane mode if you want to open  
    multiple new sites at the same time.  
    See also  
         emerald-browser  
    close  
-   ### 37. Swap  
+   ### 40. Swap  
   
    Swaps two files  
    Example  
    swap text1 text2  
-   ### 38. Exp  
+   ### 41. Exp  
   
    exp is an exponentiation tool  
    (echo 5; echo 3) | exp  
    => 125  
    (echo 2; echo 10) | exp  
    => 1024  
-   ### 39. Div  
+   ### 42. Div  
   
    Divides numbers  
    Example  
    (echo 5000; echo 100) | div  
    => 50  
-   ### 40. Mul  
+   ### 43. Mul  
   
    Multiply numbers  
    echo 1 > file  
    echo 2 >> file  
    echo 3 >> file  
    echo 4 >> file  
    echo 5 >> file  
    cat file | mul  
    => 120  
-   ### 41. Nth  
+   ### 44. Nth  
   
    Nth gets the nth line from the input  
-   ### 42. Abs  
+   ### 45. Abs  
   
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
-   ### 43. Add  
+   ### 46. Add  
   
    See the sub example  
    add adds integers from the standard input  
    (echo 1; echo 2; echo 3) | add  
    The result would be 6  
-   ### 44. Sub  
+   ### 47. Sub  
   
    Sub is a simple command line program that subtracts integers.  
    For some reason, no simple program did this.  
    Which is weird  
    Example  
    sub  
    (Input)  
@@ -839,34 +860,34 @@
    1  
    Result =>  
    6  
    Example  
    (echo 5; echo 2) | sub  
    Result =>  
    3  
-   ### 45. Rip  
+   ### 48. Rip  
   
    Replace In Place  
    rip tool replaces a string, not a regular expression, with another  
    string  
    Example  
    rip cat dog file  
-   ### 46. G+  
+   ### 49. G+  
   
    A compiler for C += 2. If you want to use C++ with Python syntax, you  
    can use this.  
    Usage is like g++  
    Example  
    g+ a.cpp -o out  
    See also README file & emerald-browser and its source  
-   ### 47. T  
+   ### 50. T  
   
    “t” is incredibly useful.  
    It can be used many, many times every day by computer power users.  
-   It is kind of like “sed”, or perl, python or ruby.  
+   It is kind of like “sed,” or perl, python or ruby.  
    It's the ULTIMATE shell “glue” tool.  
    t reads every line from the standard input, and for every line, it  
    evaluates a ruby expression  
    t a + 2  
    would add 2 to every line  
    Number automatically get converted to numbers in Ruby.  
    So one doesn't have to worry about that.  
@@ -881,15 +902,15 @@
    echo “One line” | t a while true  
    The second line, again is a Ruby expression.  
    You can have really complex expressions on the second line.  
    You can even import modules.  
    cat /usr/share/dict/words | t 'a + “ is a good word.”'  
    That processes every word in the dictionary, and says that every word  
    “is a good word.”  
-   There are other programs in this software project like “t”.  
+   There are other programs in this software project like “t.”  
    But if you do command line text filtering, t might be the best tool  
    that you will find.  
    See also  
         gsub  
    gsubip  
    .  
   
@@ -897,43 +918,46 @@
   
     Top  
     Ultimate Chat Application.exe  
     Discourse Generator.exe  
     Emerald Browser  
     Left Right.exe  
     Find Housing  
+    Prepend Each  
     Google Speak  
+    Append Each  
     Selectlines  
     Processes  
     Emeraldc  
+    Nth Word  
     Last Nth  
     Speakcat  
     Uca Cli  
     Big Num  
     Squeeze  
     Dictate  
     Prepend  
     Chat Rb  
-    Undump  
     Append  
+    Delete  
     Gsubip  
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
-    Dump  
     Args  
     Rnip  
+    Trim  
     Quot  
     Open  
     Swap  
     Exp  
     Div  
     Mul  
     Nth
```

### Comparing `democracy-1.0.29/democracy.egg-info/PKG-INFO` & `democracy-1.0.30/democracy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: democracy
-Version: 1.0.29
+Version: 1.0.30
 Summary: Trying to help with democracy, see https://github.com/gregoryc/democracy
 Author-email: Gregory Cohen <gregorycohen2@gmail.com>
 Maintainer-email: Gregory Cohen <gregorycohen2@gmail.com>
 Project-URL: Homepage, https://github.com/gregoryc/democracy
 Keywords: ai,empowerment,agi,agis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=2.0
 Description-Content-Type: text/markdown
 
 <h1 style='color: green'>Practical Self-Empowerment Utilities Covering Every Facet of Life </h1>
-      <iframe width="80%" height="600" src="https://www.youtube.com/embed/Fx9x8cArK30" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
+  
+  [![Video](https://img.youtube.com/vi/Fx9x8cArK30/maxresdefault.jpg)](https://www.youtube.com/watch?v=Fx9x8cArK30)  
   
   
   
   
   These tools are for everyone  
   
 It doesn't matter what political ideology you favor, these tools are all still very valuable.  
@@ -44,15 +45,15 @@
    There is also an idealistic make_server program that would make a very  
    fast webserver.  
    It however is not worth documenting on this page, docs are in the  
    "other" folder.  
    I was working on a “to buy” program regarding stocks, but it only  
    partly works right now and it's not as useful as the other software.  
    The find housing tool actually helped me to find housing in real life.  
-   Those aside, there are these 83 programs.  
+   Those aside, there are these 86 programs.  
    Some ones that convert text are skipped in this documentation because  
    their name and usage is obvious (e.g., color tools).  
   
 All of these programs are mostly self-contained. This is a really good thing.  
 You can use them anywhere without dependencies.  
   
    My email is  gregorycohenvideos@gmail.com and I really would like to  
@@ -110,15 +111,15 @@
   
    So I will leave a legacy. THIS MATERIAL WILL BE USED AND UNDERSTOOD.  
   
    And I will be found by AIs, assuming they continue to exist.  
   
     Democracy Github       Ruby Gem       Python PIP Package  
   
-Without further ado, here are the 83 documented programs. (The obvious usage  
+Without further ado, here are the 86 documented programs. (The obvious usage  
 ones are omitted.)  
   
    ### 1. Ultimate Chat Application.exe  
   
    ![UCA](./images/2.png)  
    There is so much potential with this program.  
    This is a non-AI chatbot. It's not based on generative AI or AI of any  
@@ -180,55 +181,61 @@
    ### 3. Emerald Browser  
   
    ![UCA](./images/3.png)  
    ![UCA](./images/4.png)  
    Emerald browser is a really powerful new browser  
    See README  
    It works based on panes.  
-   Read the documentation for “open”, “close” and also the README file.  
+   Read the documentation for “open,” “close” and also the README file.  
    ### 4. Left Right.exe  
   
    This is a tool to bring sanity to politics.  
    ![UCA](./images/12.png)  
    It gets viewpoints from the person that see the good in each political  
    side, left, right, left, right, etc.  
    It then presents all of that.  
    Hopefully this can make people more sane and less hyper-partisan.  
    ### 5. Find Housing  
   
    This is a nice tool to find housing with.  
    It is a nice, simple command line tool. You enter the minimum and  
    maximum prices, and Kijiji opens with your options.  
    This tool kind of actually helped me to find housing in real life.  
-   The default city is "Ottawa". You can easily change this.  
-   ### 6. Google Speak  
+   The default city is “Ottawa.” You can easily change this.  
+   ### 6. Prepend Each  
+  
+   Prepends a string to each line  
+   ### 7. Google Speak  
   
    Google speak is really useful. It speaks a statement using the Google  
    Translate voice, which is probably the most authoritative and  
    high-quality text-to-speech voice that exists.  
    It's kind of like “espeak” or similar tools, but it is much better.  
    You need an internet connection for it to work.  
    It is probably limited at 100 characters.  
-   ### 7. Selectlines  
+   ### 8. Append Each  
+  
+   Appends a string to each line  
+   ### 9. Selectlines  
   
    selectlines shows all nonblank lines from the input  
    Example  
    cat file | selectlines  
    (echo 2; echo; echo; echo) | selectlines  
    => 2  
    The result would be 2, with no blank lines after that  
-   ### 8. Processes  
+   ### 10. Processes  
   
    Processes lists all processes with a certain name  
    For example  
    processes sh  
    processes bash  
    processes ruby  
    processes gsub  
-   ### 9. Emeraldc  
+   ### 11. Emeraldc  
   
    The Ultimate C Preprocessor  
    I'm naming this preprocessor “Emerald C.”  
     Link  
    Howdy!  
    First, let me state that I am very much a perfectionist.  
    C is a wonderful language. C is probably the perfect programming  
@@ -251,29 +258,29 @@
    If one runs the command line preprocessor, with the “--features” flag,  
    the program shows all of its features  
    A Better C  
    C is a fantastic language. C compiles insanely fast, is the fastest  
    language there is, is very clear, is native to all systems, and is  
    useful for all purposes.  
    Some people, e.g., Bjarne Stroustrup, consider that C is “not good  
-   enough”, and make languages like C++ or D (or thousands of others)  
+   enough,” and make languages like C++ or D (or thousands of others)  
    This is not necessary.  
    There is no reason to use Python instead of C for “simple scripting  
    tasks”  
    Some functions can be used as methods  
    Makes for an excellent “scripting language” (which is really just  
    native C without things making it slow)  
    1 String Interpolation “String interplation like this #{foo} ” Calls  
    the join() function (talked about below to join strings,  
-   delim is a static global in each module called “sep”.  
+   delim is a static global in each module called “sep.”  
    Make sure you free() the string after. The string is stored in a static  
-   global variable called “last”.  
+   global variable called “last.”  
    So you could do puts(...); free(last)  
-   2 ew *i.ew “Foo”, a.ew “bar” | char* ends with another char*?  
-   3 sw *i.sw “Foo”, a.sw “bar” | char* starts with another char*?  
+   2 ew *i.ew “Foo,” a.ew “bar” | char* ends with another char*?  
+   3 sw *i.sw “Foo,” a.sw “bar” | char* starts with another char*?  
    4 == Comparison of strs, “foo” == “bar”  
    5 strip Returns pointer to string that was stripped, in place  
    6 chomp void function, chomps end of string of spaces, i.chomp or  
    chomp(i), in place  
    7 gsub Just like ruby, there is a gsub function.  
    The preprocessor detects if you use and adds -lpcre2-8 to the link  
    flags if you use it. Use $" for substitutions in argument 3 gsub(a, b,  
@@ -352,79 +359,81 @@
    Why not use Rust?  
    $ time rustc a.rs  
    real 0m0.637s  
    user 0m0.502s  
    sys 0m0.160s  
    Rust takes 0.637 seconds to compile an empty file!  
    That is not ideal.  
-   ### 10. Last Nth  
+   ### 12. Nth Word  
   
-   Last nth gets the last n lines from the standard input  
-   ### 11. Speakcat  
+   nth_word gets the nth word of each line  
+   For example  
+   nth_word 3  
+   gets the 3rd word of each line  
+   ### 13. Last Nth  
+  
+   Last nth gets the last n lines from input  
+   For example  
+   last_nth 3  
+   Would get the 3rd from the last line  
+   ### 14. Speakcat  
   
-   Speak cat is a tool like “cat”, which shows the content of files  
+   Speak cat is a tool like “cat,” which shows the content of files  
    (technically, it combines the content of files).  
    But speak cat also speaks the text.  
    Which could be useful in some circumstances.  
    It's kind of like “tee” to your ear.  
-   ### 12. UCA CLI  
+   ### 15. UCA CLI  
   
    CLI for uca app  
-   ### 13. Big Num  
+   ### 16. Big Num  
   
    ![UCA](./images/10.png)  
-   ### 14. Squeeze  
+   ### 17. Squeeze  
   
    Squeeze reads all input from stdin, then it prints it back omitting  
    argument 1 line from the front, and argument 2 lines from the back  
    Example  
    squeeze 1 1  
    This would omit the first line and the last line  
    squeeze 5 3  
    This would omit the first 5 lines and the last 3 lines  
    squeeze 2 2 [file] also works, it outputs text to file  
-   ### 15. Dictate  
+   ### 18. Dictate  
   
    Dictate opens web pages in emerald browser, or in any browser  
    (depending on the environment variable set), by you speaking, instead  
    of typing.  
    There is a mode called c_mode, that allows you to make code from  
    speaking.  
-   ### 16. Prepend  
+   ### 19. Prepend  
   
    prepend prepends input taken from the standard input to a file  
    Usage  
    prepend [file]  
    This is text to be prepended  
-   ### 17. Chat Rb  
+   ### 20. Chat Rb  
   
    This program is excellent.  
    It's essentially a mix of ChatGPT and a shell, such as bash or ZSH.  
    It has a bunch of features.  
    It can display a file or change to a folder just by mentioning it.  
    It outputs chatgpt data to an output folder in home folder and copies  
    it to clipboard  
-   To run a shell command, prefix things with “c”, such as c gcc.....  
-   ### 18. Undump  
-  
-   undump is the opposite of dump  
-   Example  
-   echo cat | dump | undump  
-   => cat  
-   echo cat | dump  
-   => “cat”  
-   echo '“cat”' | undump  
-   => cat  
-   ### 19. Append  
+   To run a shell command, prefix things with “c,” such as c gcc.....  
+   ### 21. Append  
   
    Appends text to file  
    Example  
    append file  
    This is more text to be appended  
-   ### 20. Gsubip  
+   ### 22. Delete  
+  
+   Recursively delete all files named a certain name.  
+   ### 23. Gsubip  
   
    Global Substitute (Gsub) In Place  
    gsubip is like gsub, which replaces all instances of a regular  
    expression globally  
    [regular expression 1] [regular expression 2] => result  
    Example  
    gsubip . FOO file  
@@ -433,15 +442,15 @@
    Would make all instances of “cat” “dog”  
    It is much cleaner than “sed.”  
    You don't need to have “sed” installed to run this program.  
    It doesn't read from the standard input  
    It takes exactly 3 arguments, no more, no fewer.  
    See also  
         gsub  
-   ### 21. Rhyme  
+   ### 24. Rhyme  
   
    A very powerful music generator program that doesn't use AI.  
     See this channel as an example of potential usage of this public  
    domain content  
    https://www.youtube.com/@LawrenceStevensMusic  
    The music industry is plagued with very foundational problems.  
    For starters, the quality of the discourse in music is very low, and  
@@ -449,15 +458,15 @@
    as during the era in which classical music was popular and before.  
    People aren't able to fight back, against superficiality and potential  
    deception in messages.  
    One of the greatest problems in the current world is the mainstream  
    scientific establishment, supported and upheld by mainstream academia.  
    To indicate what is already obvious, it exists in the context of a  
    legacy of authoritarianism and a lack of understanding of dynamism.  
-   It is not dynamic or forceful, the "results" of it don't change the  
+   It is not dynamic or forceful, the “results” of it don't change the  
    foundation of society. True free discourse is not supported, especially  
    in regards to the human mind and human well-being and human freedom.  
    These problems should be opposed and fought, it is self-evident that  
    this would be the best use of ones time, for it would lead to true  
    freedom.  
    One excellent way to combat this would be to use the generated songs  
    generated by a computer program called Rhyme, available at  
@@ -476,15 +485,15 @@
    Shoving art and flippant content in ones face, is the best way of doing  
    such.  
    Accountability must always be brought about.  
    Is music good and desired? For sure.  
    USAGE OF PROGRAM  
    Enter basename to make songs folder in (folder/songs, num songs =  
    13000)  
-   Usage rhyme [folder] (processes files "1.json" and "21.json" by  
+   Usage rhyme [folder] (processes files “1.json” and “21.json” by  
    default)  
    Example output of a song  
    ![UCA](./images/7.png)  
    (NO COPYRIGHT RESTRICTIONS ON THIS CONTENT WHATSOEVER. FULLY PUBLIC  
    DOMAIN)  
    Name the song or poem as you wish, resell it, but please positively  
    influence culture  
@@ -577,15 +586,15 @@
    Working don't matter for this, whether day or graveyard  
    They don't care about your feelings, they don't regard  
    They are failures, down at the boulevard  
    They don't have decency, they automatically disregard  
    They're a complete failure, they only neglect  
    They don't speak the language of the people or their dialect  
    This is not right, this is completely incorrect  
-   The only focus on “responses”, they just want to deflect  
+   The only focus on “responses,” they just want to deflect  
    The lies are put forth, the lies they erect  
    CHORUS  
    They're such failures, themselves they outdid  
    Cutting out the conversation, putting on the lid  
    Don't have to do with ego or id  
    Running away from conversation just like a kid  
    Their neglect is out of this world, I swear it's avant-garde  
@@ -614,56 +623,55 @@
    Their sucked in their circle, they never wave  
    Away from the truth, on the outskirt  
    With pre-thought of ideas, they automatically assert  
    Any progress is fleeting with them, they revert  
    Disingenuous to the extreme, the society they subvert  
    The society is the ones who hurt  
    ---  
-   ### 22. Email  
+   ### 25. Email  
   
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
-   ### 23. Floor  
+   ### 26. Floor  
   
    Gets the floor of numbers e.g. 21.3 -> 21  
-   ### 24. Rgsub  
+   ### 27. Rgsub  
   
    Recursively replaces text.  
    Verbosely tells you everything that happens.  
    Non-regex.  
    Example  
    rgsub my_email@site.com my_second_email@site.com  
    Would replace an email recursively in a directory.  
    It tries to skip non-text files and hidden files.  
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~  
-                Usage: rgsub   [optional list of files instead of recursive sear  
-ch]  
-                If a file is "-" or stdin, read from stdin and output to stdout.  
-                Options  
-                    -r, rename files instead of replacing contents of files.  
-                        find and replace in file and dir names instead  
-                    -v, verbose mode  
-                    -- Indicate end of options.  
+        Usage: rgsub   [optional list of files instead of recursive search]  
+        If a file is “-” or stdin, read from stdin and output to stdout.  
+        Options  
+        -r, rename files instead of replacing contents of files.  
+        find and replace in file and dir names instead  
+        -v, verbose mode  
+        -- Indicate end of options.  
   
-   ### 25. Lines  
+   ### 28. Lines  
   
    Lines gets the number of files in the current folder that you are in.  
    It can also act like “wc -l” if you pipe data into it.  
-   ### 26. Clock  
+   ### 29. Clock  
   
    clock is useful  
    clock is a command line alarm clock  
    It wakes you up at 8:14, or at a time specified  
    Usage  
    clock  
    Runs clock  
@@ -672,22 +680,22 @@
    clock 9 0  
    Sets an alarm clock for 9 in the morning  
    It uses flite to wake you up  
    It speaks with a bunch of voices  
    To stop it  
    Run this command  
    clock stop  
-   ### 27. Emoji  
+   ### 30. Emoji  
   
    Emoji converts words to emojis from the standard input  
    It can also speak the output  
    It can also copy the output to your clipboard  
    It is very useful  
    ![UCA](./images/6.png)  
-   ### 28. Close  
+   ### 31. Close  
   
    “Close” is a simple program that closes “Emerald Browser,” a new web  
    browser based on the same engine as Chrome. Currently, Emerald Browser  
    only works on Linux and Mac (Or Windows with Windows Subsystem for  
    Linux or a Virtual Machine, but getting it to work might be tricky).  
    “close” closes the Web Browser, which is normally full-screen.  
    More accurately, it kills the browser, and all other copies of Emerald  
@@ -713,75 +721,70 @@
    Emerald browser has a built in the top. The terminal is the navigation  
    bar.  
    Some more work needs to be put into the browser.  
    Currently, new tabs can't be opened, which might be a dealbreaker for  
    some people.  
    Currently, content, like YouTube videos, can't be made fullscreen.  
    If anyone wants to contribute, feel free to!  
-   ### 29. Copy  
+   ### 32. Copy  
   
    copy copies the standard input  
    Example  
    ls | copy  
-   ### 30. Gsub  
+   ### 33. Gsub  
   
    Gsub is very powerful.  
    Usage  
    gsub [regular expression] [replacement text]  
    Example  
    cat text | gsub man dog  
    cat text | gsub 'man|boy|cat|dog' food  
    ls | gsub Desktop cat  
-   ### 31. News  
+   ### 34. News  
   
    Gets the news from bbc  
    Usage  
    news  
    news speak  
    uses google_speak to SPEAK the news, one story at a time.  
    ![UCA](./images/5.png)  
-   ### 32. Dump  
-  
-   Dump surrounds its input with quotes  
-   ls | dump  
-   => “....”  
-   Use undump to get the reverse  
-   See also  
-        undump  
-   ### 33. Args  
+   ### 35. Args  
   
    args is like a better xargs  
    args works properly with spaces in the name of commands  
    It takes exactly one argument  
    Example  
    ls | args “mv -t ../f”  
-   ### 34. Rnip  
+   ### 36. Rnip  
   
    Replace Not In Place  
    This is like gsub, but for strings, not for regular expressions  
    Example  
    echo .......... | rnip foo bar  
    See also  
         gsub  
-   ### 35. Quot  
+   ### 37. Trim  
+  
+   Trims spaces of each line  
+   ### 38. Quot  
   
    Turns quotes in text into good text and makes text presentable.  
    Example  
    $ echo 'Joe said,        "One two three".' | quot  
    Joe said, “One two three.”  
    Example 2  
    quot < essay  
    Example 3  
    (Quote the file and output it)  
    quot text_file  
-   ### 36. Open  
+   ### 39. Open  
   
    “open” is a very efficient program that searches a query from google,  
    and then opens it in Emerald Browser.  
-   If you ever want something to “just open”, you can use it.  
+   If you ever want something to “just open,” you can use it.  
    Example  
    open “cats”  
    An earlier version of open worked like this  
    open [site1] [site2] [site3] N  
    site1, site2, and site3 would all be opened, and the top N queries were  
    all shown in different panes  
    An even earlier version of this program used Chrome to open the sites.  
@@ -790,65 +793,65 @@
    open “cats” “dogs” “frogs”  
    All of those queries would open in Emerald Browser.  
    Just make sure it is compiled in multipane mode if you want to open  
    multiple new sites at the same time.  
    See also  
         emerald-browser  
    close  
-   ### 37. Swap  
+   ### 40. Swap  
   
    Swaps two files  
    Example  
    swap text1 text2  
-   ### 38. Exp  
+   ### 41. Exp  
   
    exp is an exponentiation tool  
    (echo 5; echo 3) | exp  
    => 125  
    (echo 2; echo 10) | exp  
    => 1024  
-   ### 39. Div  
+   ### 42. Div  
   
    Divides numbers  
    Example  
    (echo 5000; echo 100) | div  
    => 50  
-   ### 40. Mul  
+   ### 43. Mul  
   
    Multiply numbers  
    echo 1 > file  
    echo 2 >> file  
    echo 3 >> file  
    echo 4 >> file  
    echo 5 >> file  
    cat file | mul  
    => 120  
-   ### 41. Nth  
+   ### 44. Nth  
   
    Nth gets the nth line from the input  
-   ### 42. Abs  
+   ### 45. Abs  
   
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
-   ### 43. Add  
+   ### 46. Add  
   
    See the sub example  
    add adds integers from the standard input  
    (echo 1; echo 2; echo 3) | add  
    The result would be 6  
-   ### 44. Sub  
+   ### 47. Sub  
   
    Sub is a simple command line program that subtracts integers.  
    For some reason, no simple program did this.  
    Which is weird  
    Example  
    sub  
    (Input)  
@@ -857,34 +860,34 @@
    1  
    Result =>  
    6  
    Example  
    (echo 5; echo 2) | sub  
    Result =>  
    3  
-   ### 45. Rip  
+   ### 48. Rip  
   
    Replace In Place  
    rip tool replaces a string, not a regular expression, with another  
    string  
    Example  
    rip cat dog file  
-   ### 46. G+  
+   ### 49. G+  
   
    A compiler for C += 2. If you want to use C++ with Python syntax, you  
    can use this.  
    Usage is like g++  
    Example  
    g+ a.cpp -o out  
    See also README file & emerald-browser and its source  
-   ### 47. T  
+   ### 50. T  
   
    “t” is incredibly useful.  
    It can be used many, many times every day by computer power users.  
-   It is kind of like “sed”, or perl, python or ruby.  
+   It is kind of like “sed,” or perl, python or ruby.  
    It's the ULTIMATE shell “glue” tool.  
    t reads every line from the standard input, and for every line, it  
    evaluates a ruby expression  
    t a + 2  
    would add 2 to every line  
    Number automatically get converted to numbers in Ruby.  
    So one doesn't have to worry about that.  
@@ -899,15 +902,15 @@
    echo “One line” | t a while true  
    The second line, again is a Ruby expression.  
    You can have really complex expressions on the second line.  
    You can even import modules.  
    cat /usr/share/dict/words | t 'a + “ is a good word.”'  
    That processes every word in the dictionary, and says that every word  
    “is a good word.”  
-   There are other programs in this software project like “t”.  
+   There are other programs in this software project like “t.”  
    But if you do command line text filtering, t might be the best tool  
    that you will find.  
    See also  
         gsub  
    gsubip  
    .  
   
@@ -915,43 +918,46 @@
   
     Top  
     Ultimate Chat Application.exe  
     Discourse Generator.exe  
     Emerald Browser  
     Left Right.exe  
     Find Housing  
+    Prepend Each  
     Google Speak  
+    Append Each  
     Selectlines  
     Processes  
     Emeraldc  
+    Nth Word  
     Last Nth  
     Speakcat  
     Uca Cli  
     Big Num  
     Squeeze  
     Dictate  
     Prepend  
     Chat Rb  
-    Undump  
     Append  
+    Delete  
     Gsubip  
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
-    Dump  
     Args  
     Rnip  
+    Trim  
     Quot  
     Open  
     Swap  
     Exp  
     Div  
     Mul  
     Nth
```

### Comparing `democracy-1.0.29/pyproject.toml` & `democracy-1.0.30/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "democracy"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.29"  # Required
+version = "1.0.30"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Trying to help with democracy, see https://github.com/gregoryc/democracy"  # Optional
 
 # This is an optional longer description of your project that represents
```

