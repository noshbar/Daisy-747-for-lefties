# Left-handed Daisy 717/747 grips

![Current result](blog/result.jpg)

## TL;DR;
Download `left-grip.stl` and 3D print it.
Check out the Blender files in `sources` if you want to edit anything.
**NOTE**: this is a **WIP**, not perfect yet.

## Blog

I recently bought a second-hand [Daisy 747 air pistol](https://www.pyramydair.com/s/m/Daisy_Match_Grade_Avanti_747_Triumph_Match/308) with the intent of becoming an Olympic-quality target shooter.

I really like it, but it wasn't built for *sinister* people like me.
This is due to the existing left grip being specially shaped to house the thumb of the right hand.

I searched near and far online for lefty replacements, but alas, no left-handed dice.
So I decided to remake the grips for lefties, or at the very least, a mirrored version of the right grip for the left (for now).

And seeing as I never ever do something even remotely properly, I'm putting this out into the world so I can at least try and shame myself into making a tiny bit of an effort (and [Thingiverse](http://www.thingiverse.com) just isn't working for me).

I've never used photogrammetry before, nor have I tried replicating a real-world object, so below lie the details of my misadventures.

#### Update 1

![Current result](blog/photogrammetry01.jpg)
screenshot of the photogrammetry result, available in `sources/photogrammetry01.blend`

I took 30 poorly-lit photos of the existing grips and shoved them into [MeshRoom](https://alicevision.org/#meshroom), which only took a few minutes to give me a really gross point cloud.

From there, I imported the `OBJ` into [Blender 2.8](https://www.blender.org/) and removed a bunch excess points to make things a little more responsive. The screenshot above is the result of that process.

![Box base](blog/boxbase.jpg)

Above is my first attempt at box sculpting.
I started with a cube, extruded it a few times, trying to match the outline of the sides first.
After that I made a loop cut (`CTRL-R`), increasing the amount of cuts a few times (mousewheel up) so I could get some more detail following the shape.

From there I simply grabbed the top vertices one by one, and lowered them until I just wasn't seeing any of the photogrammetry mesh peeking through (well, except the bottom bits, did I mention I don't do anything in my spare time properly?).

With that done, I added a subsurface modifier -2 levels- and used a boolean-cube to cut the bottom of my subsurface flat.

It was printing time!
0.3mm layers, 10% infill, go Anycubic i3 Mega, go!
*Side note: I really really like the Mega. I've printed 2 spools worth of stuff on it so far, and it hasn't failed once.* 

![Attempt #1](blog/attempt01.jpg)

Success-ish!
I somehow buggered up the vertical scale, and I kinda forgot to put a hole in the back, but nothing a bit of tracing and drill bits can't solve!

Teething and hand pains aside, it actually works!