# Stage-Intro
Attached character for the IKEMEN engine. Makes fancy stage intros more usable.

![CvS](https://github.com/RealFoobs/stage-intro/blob/main/cvs.gif)

# How to use
Place the "intro" folder in `\stages`.

Open the stage you wish change on any text editor and look for the `[Info]` section. Add the following line:

```
attachedchar = Intro/Intro.def
```

Afterwards, create a new section below it called [Constants] with this information:

```[Constants]
intro_startup = 180
```
180 is a placeholder value; change it to however long you need the characters to be frozen before their intros start, in ticks (60 ticks = 1 second). There's no one size fits all since every stage has different animations and bgctrls, but 180 is a good place to start if you're eyeballing the duration of the intro.

# Note:
Some stages have wonky looping in Survival mode, missing some or all of the intro elements after the first fight. This is no fault of my code, which will pause all the playable characters under the assumption everything is working as intended.
