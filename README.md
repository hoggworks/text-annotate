# text-annotate
Select HTML text to generate multiple dynamic underlines. R&amp;D.

The goal of this was to see if I could create a system that would let me underline text by selecting it, and if I could have multiple overlapping underlines of said text. This was related to an idea for a debate website that never materialized, where people would be able to select text from an item being debated, and use that to branch off a discussion. 

The usage of this is super-simple: just click and drag your mouse over the text; when you let go, a highlight in one of a handful of randomly selected, pre-defined colours will get added. And they stack. It's a neat visual effect that might be helpful to someone. 

### Usage ###
Copy all JS and CSS into your new project. 
Presently the code will draw out any text defined as init_text. So change that to your desired code, and then load the page. At present, text-annotate doesn't support any HTML formatting. 

### Shortcomings ###
Due to a limitation of JS, I wasn't able to get it to know **where** in a block of text you're highlighting; all the browser can know is what you're selecting. As such, if you select an element of text that exists earlier in the block (if a phrase is repeated, or if you select a simple word of word fragment like "you" or "ou"), text-annotate will get confused and think the earlier instance of the selected text is the appropriate one.


### TODO ###
Encapsulate the code so that it'll support multiple blocks of text.
Separate files, make it look pretty.
Consider remaking this using the Canvas tag, if that allows for greater control.
