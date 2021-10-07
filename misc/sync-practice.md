1. Consider the following scenario involving two processes.

```c
// shared
semaphore sem = 1

// Code for proc 0
wait()
signal()
signal()
wait()
wait()
wait()
signal()
signal()
signal()
...
```
```c
// Code for proc 1
wait()
signal()
...
```

What are the possible outcomes?

2. A toy is produced in a two-step assembly process.

The first machine in the process has unlimited raw materials available to it.
When it finishes its part of a toy,
a moving track brings the base-toy to an intermediate storage room.

The second machine draws one base-toy at a time from the intermediate storage
room and produces one completed toy that is then sent out of the factory.
There are an unlimited number of trucks ready to take away toys as fast as they
can be produced.

The intermediate storage room has some extra space in case the first machine
gets slightly ahead of the second.
It can hold five base-toys at a time.
If the first machine tries to put six toys in the room,
the track collapses and the factory cannot work.
If the second machine tries to pull a base-toy when one is not there,
it explodes and all of the robot workers are sad.

Write code for the two machines to control this process.

You can assume functions like `create_base_toy`, `push_to_intermediate_room`,
etc. are already available to you.

Remember -- the goal of the factory is to produce as many toys as possible to
make a profit,
so try to allow as much work as you can at once
(i.e., a "lock-step" solution is not ideal).

3. Consider the same situation as the previous problem,
but the factory is now making toys in three steps.

There is still an intermediate room between the first two steps that can hold
five items.
There is now an additional intermediate room between steps two and three that
can hold three items.

Write code for each machine that will allow the factory to run smoothly.

4.  Assume you have an art gallery with unlimited seating capacity
(isn't math great?).
People come in from the street, view the art, and leave.

However, there is a disease called DIVOC spreading rapidly through the town. 
People infected with DIVOC are allowed to enjoy the gallery,
but only one at a time, and no healthy patrons may be present.

Write separate code for DIVOC-infected people and healthy people to determine
how they access the gallery.

You may assume functions such as `enter_gallery`, `view_art`, etc. are
available to you.

5. Consider the same art gallery situation as before.
However, the CDC has recently determined that it is safe for DIVOC-infected
people to be together as long as no non-infected people are present.

So, the gallery is now allowing in an unlimited number of DIVOC-infected
patrons as long as no non-infected patrons are present.

Write the code for controlling patron behavior according to these rules.
Consider whether your solution allows for starvation.
The most "natural" solution will, which is fine in this case.

6. Consider the art-gallery situation.
The CDC has changed its mind,
and now only one DIVOC-infected patient is allowed in at once,
just as in the initial scenario.

However, the gallery manager was complaining about your previous solution.
Surprisingly, it turns out that there was not unlimited space in the gallery.
In fact, the gallery can comfortably hold at most four patrons at once.

Write new code for controlling patron behavior.

7. Consider a tennis club run by a strange and not-very-bright person.
Each player requires a hat, racquet, and ball before they can begin playing.
Players are only allowed to use goods checked out from the club.

The club has just four each of hats, racquets, and balls.
Because of the rules,
there are always more people waiting to play than resources available.
Each person may grab the resources in any order,
but they can grab just one at a time.

Write code to determine how person `i` should acquire their resources to make
this process as smooth as possible.

You may assume that every person already has a pro waiting on the court to hit
with them.
So, as soon as they have there materials,
their game can begin.

Note: avoiding deadlock is an important goal in any solution.
However, for this problem,
it may be more interesting to consider ways that you can "acheive" deadlock
than ways that you can avoid it.
