# Week 8: Lab Report 4

[Link of my own code][1]

[Link of the code I reviewed][2]

[1]: https://github.com/xiuyuan0216/markdown-parse.git

[2]: https://github.com/clingunis/markdown-parse.git
## Snippet 1

> The following is the markdown preview of Snippet 1:

<img src = "3BB967FF-BC71-41CC-8EDE-091D9079B9A4.jpeg" width = "500" height = "300">

> We see that url.com is not counted as a link by markdown. Therefore, the links should be 'google.com, google.com, and ucsd.edu. My test method is as follows.

<img src = "CE3A1A61-1502-4240-870E-C6E284311139_4_5005_c.jpeg" width = "500" height = "300">

> Then the following picture is the Junit output of my code.

<img src = "F8A591EF-5BD0-4096-8B31-BDC03C1055F4_4_5005_c.jpeg" width = "500" height = "300">

>The following picture is the Junit output of my code. It is basically the same as the output of my code.

<img src = "F8A591EF-5BD0-4096-8B31-BDC03C1055F4_4_5005_c.jpeg" width = "500" height = "300">

> I don't think a small change can make my program work for Snippet with inline backticks. Only the open bracket cannot be surrounded by a pair of backticks. It is okay for close paren to have a pair of backticks surrounded. Therefore, it is very difficult to use small changes to handle these different cases. A more involved change is needed.


## Snippet 2

>The following is the markdown preview of Snippet 2:

<img src = "B029FABD-0F34-4413-A838-CF73573C26F3.jpeg" width = "500" height = "300">

> As we can see, for nested links, the outer b.com is not counted by markdown as a valid link. Therefore, the links should be a.com, a.com(()), and example.com. My test method is as follows.

<img src = "241E476B-913F-4988-866A-1C47BDF5692F_4_5005_c.jpeg" width = "500" height = "300">

>Then the following picture is the Junit output of my program:

<img src = "5DA12764-0839-4779-BB51-F30C353B220C_4_5005_c.jpeg" width = "500" height = "300">

>The following picture is the Junit output of the program I reviewed:

<img src = "5DA12764-0839-4779-BB51-F30C353B220C_4_5005_c.jpeg" width = "500" height = "300">

>I don't think a small change to my code can solve this problem. For nested parentheses, except the outer pair of parentheses, others are regarded as part of the link. Here, a stack should be used to handle this kind of situation, and that would be totally different code from our current MarkdownParse.


## Snippet 3

>The following picture is the markdown preview of Snippet 3:

<img src = "8F11F9E3-93B8-4702-BCE5-11517A3EEDC4.jpeg" width = "500" height = "300">

> As we can see, there should not be an empty line inside brackets or parentheses. Therefore, only https://ucsd-cse15l-w22.github.io/ is counted by markdown as a valid link. My test method is as follows:

<img src  = "FEB31045-C844-4F9C-A5BF-BC734CDDBCEA_4_5005_c.jpeg" width = "500" height = "300">

>Then the following is the Junit output of my own program:

<img src = "86841A1A-33B9-4A84-9F12-5084FA2D5E60_4_5005_c.jpeg" width = "500" height = "300">

> The following is the Junit output of the program I review:

<img src = "86841A1A-33B9-4A84-9F12-5084FA2D5E60_4_5005_c.jpeg" width = "500" height = "300">

>I don't think a small change can solve this problem. We should add some codes to examine whether there is empty lines within brackets and parentheses. We should also check whether there is space before and in the link. These tasks cannot be well dealt with by using merely small changes.