testing
there is something about the collisions that doesn't work

possibly caused when a 0 is touching a wall like this
[0,x,0,0] we haven't clearly given a condition for when an element is zero
like we did for x.

figuring out how these custom hooks work is the tricky part.

They work like the useState hook, except they have more complicated operations inside them.
Used when we have more than one factor that alters the current state of a variable.

Note how useStage actually has a useState inside. The [stage] and [setStage] in line 5.

It's calling a function from another js file, gameHelpers.js.  gameHelpers.js defines the dimensions of the playable stage.

useStage is changing the state of [stage] within the dimensions defined by the createStage function in gameHelpers.