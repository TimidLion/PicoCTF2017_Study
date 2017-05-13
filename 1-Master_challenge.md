# Level 1 [Web]  
**Name** : Master Challenge
**Point** : 50
**Problem** : I really need to login to this website, but the developer hasn't implemented login yet. Can you help?  
(website : http://shell2017.picoctf.com:37907/)  
**Hints** : 
+ Where does the password check actually occur?  
+ Can you interact with the javascript directly?  

## Write up :  
Press F12.(Open Developer tool)
You can find /static/client.js file.(see it http://shell2017.picoctf.com:37907/static/client.js)
There is function validate() which return false.
However, the function make_ajax_req(input) gets 'res' as an input by "res=validate(pword)".
Which means we need to make res as an pword itself rather than false value.
In developers tool, we can use CONSOLE!
In the console, we can defile function validate again!
In console type like below.

```bash
function validate(pword){
  return pword;
}
```
Then type anything you want as an input value.
Then flag comes out!

**Date** : 2017.05.14
