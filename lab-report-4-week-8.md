Link to my markdown-parse repository: 

https://github.com/NickAzp/markdown-parser

Link to the one I reviewed in week 7:

https://github.com/lithicarus/markdown-parser

What each tests should produce based on VScode Preview:

 # Snippet 1:
  
  ![Image 1](Snippet1Preview.png)
  
  [a link](url.com)

  another link`

  cod[e

  code]
  
  getLinks should return an ArrayList of type String with the elements {"`google.com","google.com","ucsd.edu"}
  
 # Snippet 2:
  
  ![Image 2](Snippet2Preview.png)
  
  [a nested link](b.com)

  a nested parenthesized url

  some escaped [ brackets ]
  
  getLinks should return an ArrayList of type String with the elements {"a.com","a.com(())","example.com"}
  
 # Snippet 3:
  
  ![Image 3](Snippet3Preview.png)
  
  [this title text is really long and takes up more than one line

  and has some line breaks]( https://www.twitter.com )

  this title text is really long and takes up more than one line

  [this link doesn't have a closing parenthesis](github.com

  And there's still some more text after that.

  [this link doesn't have a closing parenthesis for a while](https://cse.ucsd.edu/

  )

  And then there's more text
  
  getLinks should return an ArrayList of type String with the elements {"https://www.twitter.com", "https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule", "https://cse.ucsd.edu/"}
  
 # The code in MarkdownParseTest.java for turning each snippet into a test is below:
  
  ![Image 4](Teststatements2.png)

 # The result of my implementation for the snippets is below:
 
 ![Image 5](Mine.png)
 
 # The result of the implementation I reviewed for the snippets is below:
 
 ![Image 6](Theirs.png)
 
 # Possible code changes for my implementation:
  For Snippet 1:
  
  I think it would take more than 10 lines to fix this change. I believe my code may have gotten messed up from the extra spaces as well as the backticks, and my current code uses indexing from the brackets. I would need to change indexing and account for backticks in the link as well as 
  
  For Snippet 2:
  
  I also think it would take more than 10 lines to fix this change. I use the indexing of parathesis and brackets in combination to currently find what's inside of them, so extra parathesis or brackets may cause my code to misfunction. Additionally, the extra spacing in this snippet is uncounted for in my code.
  
  For Snippet 3:
  
  My code accounts for the link to be on one line for the indexing, which would cause issues when the link is on multiple lines, link in this snippet. Even the name of the link might also cause issues if it's on multiple lines. These issues with the added problem of extra new lines would mean that it would take more than 10 lines to fix my code for this snippet.
