# Snake
![Game screenshot](screen.png)
A basic little snake game.  Eat as many green squares as you can before dying.  Don't touch your tail or the edges of the screen!

Built with [termloop](https://github.com/JoelOtter/termloop), and made over a weekend as part of the [codelympics Go Game Jam](https://codelympics.io/projects/2).  This repository is preserved for posterity; further development will take place in a [new repo](https://github.com/jodizzle/gosnake).

# Play

Install:
```bash
$ go get -u github.com/jodizzle/snake
```
Run:
```bash
$ $GOPATH/bin/snake
```
(gameplay tested on Linux and Windows)

# Game Jam Post-Mortem
Even though I probably had enough time this weekend, I made the mistake of spending of lot of time reading about Go and walking through tutorials instead of working on the product.  This lead me to dwindle my grand, magnificent vision for an amazingly perfect game (some sort of RPG-Roguelike-Action-Adventure-FPS, I think?) to something a little more tepid.  Since I've never actually programmed snake, I thought I'd give it a shot.  I think the project turned out pretty well and was a good first Go-effort, though I suspect the code doesn't look very much like Go is supposed to look.  I rushed on the organization (it would be worth splitting into multiple files) and skipped some abstraction in the name of time constraints.  The project definitely deserves some cleaning up.

Working with Go for the first time was fun!  It's been a little while since I've worked with a statically typed language, and I liked the readable style that the language encouraged — not that, again, this project is super exemplary of that.  I got tripped up at one point by pointers (and trying to mutate some of the elements of an array in place inside a loop, but that part is more embarassing), but everything went fairly smoothly.

[Termloop](https://github.com/JoelOtter/termloop) was effective for what I wanted to do after playing with it while reading through the examples and parts of the source.  I ran into an annoying problem with a collision condition inexplicably activating when it seems like it shouldn't have, but I was able to develop a workaround.  A bigger concern is performance: I'm using a tiny underpowered laptop, but even so, my game seems like it is more taxing than it ought to be.  Something to look into.

Overall, this was a great experience.  I hope to continue working on this and similar projects in the future.