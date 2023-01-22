# download-facebook-messages

way to download messages between you and someone else  
  
\-first you need to go [http://m.facebook.com/messages/](http://m.facebook.com/messages/)  
\-Then click the person you want to see the first message with.

Now press <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>J</kbd> and then paste this code into the lower window that pops up, and then press <kbd>Enter</kbd>. It will then proceed to load old messages until it reaches the very first message. Here is the code:

```
setInterval(function () {
document.getElementById('see_older')
.getElementsByClassName('content')[0].click();
}, 500); 
```

The above code can also be found on this website: [http://jsfiddle.net/magicramki/k9gda3cu/](http://jsfiddle.net/magicramki/k9gda3cu/)

If you do not want to go back all the way, you will need to stop the script. In order to do that, you will first need to define it as a variable:

```
var myVar=setInterval(function () {
document.getElementById('see_older')
.getElementsByClassName('content')[0].click();
}, 500); 
```

Then to stop it, you will simply need to enter the following command:

```
window.clearInterval(myVar)
```

You can resume the script anytime by typing the first part again.

Now once it loads everything, You can right click anywhere on the page and choose "save as" and then save that file somewhere on your computer. Then use Google Chrome to open it when you want to view it later (won't look right in Internet Explorer). This will save the entire chat, complete with pictures and emoticons. When you want to search for a particular day, press <kbd>Ctrl</kbd>+<kbd>F</kbd> to bring up the find box. Then type in "Mar 2", for example, to bring up the conversation on March 2nd.
