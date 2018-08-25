## Readability over brevity

Writing maintainable code is a different than solving a coding challenge in sixty lines or less.  Always aim for readability so that your code can better be understood and maintained without any further consult from you the author.  If you're having to maintain communications (asynchronous or worse synchronous <- yikes!) to advise and explain what you meant once upon a time, you'll begin to see the value of readability.  If YOU come back to your own code and no longer understand it, it's time to check yourself (and probably refactor that code to make it more expressive and readable...and maintainable...and understandable...and -insert so many other synonyms here that are all good things-).

Of course, you say.  Why wouldn't I?

Brevity.  Brevity itself is also generally a good thing.  We're taught to be concise.  We're taught to keep things short, lines < 100 characters, files < 100 lines, etc.

So brevity can be an end in itself, but when you choose it over readability, you should take pause - it's usually the wrong decision.

Often there's a balance that can be struck here.  Consider variable names.

`x = 3`

By itself, we wonder what `x` is, why it was declared, what purpose it will serve.  Probably no one would argue that...

`counter = 3`

is an improvement.  Now we get it.  A loss of brevity we could probably all get behind.  But now, what about...

`suchAndSuchWidgetLoopCounterGettingResetToZeroWheneverGroceryCartIsEmpty = 3`

Wow that's a lot of information.  On the plus side, I'm learning a lot about the surrounding code without even looking at the surrounding code.  But am I still being concise?  Moreover, did I actually improve the readability of the code?  No, it actually became less readable as my brain is having to spend the time reading and digesting the name of this variable only to obtain information quickly gleaned from looking at the surrounding code (assuming that code is at least marginally readable).

TODO