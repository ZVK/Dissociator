Dissociator.js
translated to Javascript in 2013 by ZVK @ dadabots.com || drawordoodle@gmail.com

based on Dissociated-press.php by David Pascoe-Deslauriers <dpascoed@csiuo.com>
Here's how the algorithm works:
1. Break up the corpus into a series tokens, in my case words and spaces.
2. Jump to a random token.
3. Select the 3 next tokens and output them.
4. Find the other occurrences of those 3 tokens in the corpus. Randomly select one of those occurrences and jump to that location in the text.
a. If 2 or less occurrences are found, jump to a random token instead to avoid loops.
5. Repeat steps 3 and 4 until we've outputted enough.