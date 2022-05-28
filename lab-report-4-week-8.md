Link to my markdown-parse repository: 

https://github.com/NickAzp/markdown-parser

Link to the one I reviewed in week 7:

https://github.com/lithicarus/markdown-parser

What each tests should produce based on VScode Preview:

  #Snippet 1:
  
  ![Image 1](Snippet1Preview.png)
  
  [a link](url.com)

  another link`

  cod[e

  code]
  
  getLinks should return an ArrayList of type String with the elements {"`google.com","google.com","ucsd.edu"}
  
  #Snippet 2:
  
  ![Image 2](Snippet2Preview.png)
  
  [a nested link](b.com)

  a nested parenthesized url

  some escaped [ brackets ]
  
  getLinks should return an ArrayList of type String with the elements {"a.com","a.com(())","example.com"}
  
  #Snippet 3:
  
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
  
  #The code in MarkdownParseTest.java for turning each snippet into a test is below:
  
  ![Image 4](Teststatements2.png)

  The Result of my 
  
 
