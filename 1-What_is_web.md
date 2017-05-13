# Level 1 [Web]
**Name** : 'What is web'
**Point** : 20
**Problem** : Someone told me that some guy came up with the "World Wide Web", using "HTML" and "stuff". Can you help me figure out what that is? Website.
(website link : http://shell2017.picoctf.com:52334/)
**Hints** : + How can you figure out how the webpage is actually built?

## Write up : 
Pressed F12 in Chrome. (Open Development tool)
First part of flag is in the HTML file.
Second part of flag is in the hacker.css file.(see it by http://shell2017.picoctf.com:52334/hacker.css)
Third part of flag is in the script.js file.(see it by http://shell2017.picoctf.com:52334/script.js)

The flag is concatenation of three parts of original flag.

**Date** : 2017.05.14
