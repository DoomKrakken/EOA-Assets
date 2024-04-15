MISTER XEOTROID'S AMAZING LOOPING SOUND TECHNIQUE #1

Loops often consist of three parts - start, loop and stop - and they are usually separate. That's a bit of a mess to make work nicely with ZDoom without having to make redundant and ugly coding (at least with Decorate, I have zero experience with ZScript).
So, I combined the Start and Loop sounds into one and added a loop tag to it, supported natively by ZDoom. For instance, if you want to make the Mancubus's continous flamethrower sound cool, you can start the attack state with a PlaySound that will play the combined start-loop sound and after getting to the end of it, it will loop back from only the loop is supposed to start.
Then, when you're done, you just play the stop sound on the same channel. This way, you have one nice sound, with no cut off and pretty much just two lines of code (I think it had to be a bit hacky to play the start and loop sounds separately)

If this is nothing new to you, sorry for wasting your time. :D