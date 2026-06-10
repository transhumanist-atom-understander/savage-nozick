# Newcomb's problem from the grand-system and petty-system views

It's pretty easy to do quantum mechanics every day and never think about interpretations.
For example, using quantum chemistry software.
You input a molecule as a file with a row for each atom, with the atom's element identity and xyz coordinates.
Just the atoms in the molecule, which represents a molecule floating in empty space, which is fine for gas phase properties.

You can do some impressive calculations with modern software.
Erwin Schrödinger could calculate the hydrogen atom spectrum, but with a computer you can compute which frequencies of light will be absorbed by, for example, organic pigments used to dye clothes or as food colorings.
Of course for a dye you don't want the color of a gas but of a solution in water or another solvent, but this can be approximated without explicitly including the solvent molecules by just adjusting the vacuum permittivity with the solvent's dielectric constant.

So, I'm used to working with explicit atom-by-atom models, and thinking of quantum mechanics as a program that operates on such models.
It's only when reading blog posts, not when doing quantum mechanics, that I consider the fundamental object of quantum interpretations: the joint quantum state of the molecule and the experimenter.

It's more than just that I don't have an atom by atom description of the experimenter, more than just that a human body has too many atoms for the software to handle.
Returning to the question of whether a molecule absorbs a certain frequency of light, one way to frame such calculations is to model the light as an oscillating electric field, and check if the expected energy of the molecule goes up.
So I'm not even including the measurement device, just indirectly inferring that less light energy reaches some "off-screen" measurement.
But I'm not specifically _excluding_ the measurement device either.
I mean, I don't even include the solvent.
So what I feel is not a Cartesian boundary between mind and matter, but a much tighter boundary around what's explicitly modeled.

## Decision theory when you're used to explicit models

I think you can also use what I'll call "classical decision theory", for which my reference is Savage, and never worry about Newcomb's problem, for similar reasons.
[Savage's book](https://archive.org/details/foundationsofsta0000sava/page/n1/mode/1up), as philosophical as it is, only makes sense to me when I read it from the perspective I've developed for explicit modeling.
In his theory, an "act" is a function that maps from a state of the world to a consequence.
Savage explains that by "the world", he means "the object of interest".
For example, in the decision problem of what to do with an egg that may or may not be rotten, the world is the egg.
Readers concerned that this may be too narrow a conception of "the world" will find that he goes on to consider: "if the person is interested in the only brown egg in a dozen, should that egg or the whole dozen be taken as the world?"

In [Nozick's paper introducing Newcomb's problem](https://philpapers.org/rec/NOZNPA), he thinks the world really means the whole world, which creates some interesting miscommunications with the classical theory.
What Nozick calls a "state of the world" is in Savage's theory a (state, act) pair.
This makes sense if you consider "the world" to include yourself.

I don't think Savage even realizes that his formalism requires leaving the decider out of the world.
After the dozen eggs, he does consider that the state of the world may be the "exact and entire past, present, and future history of the universe", but his objection to this is that it is "vague", and:

> It may also be added that the use of modest little worlds, tailored to particular contexts, is often a simplification, the advantage of which is justified by a considerable body of mathematical experience with related ideas.

It's true that if you want to actually derive consequences from explicit models, then you're used to simplifying to the bare minimum.
Perhaps that makes it easy to miss that including yourself in the model introduces special problems, since for the sake of simplification you don't get anywhere near including that much.

## The appeal of the grand systems perspective

In [his original paper on what we now call the "many-worlds" interpretation](https://doi.org/10.1103/RevModPhys.29.454), Everett motivated it with quantum cosmology, since there's nowhere outside the universe for a Copenhagen-style observer to stand.
Eliezer Yudkowsky said something similar to motivate timeless decision theory:

> I hold it a virtue of any decision theory that it should be compatible with a grand-system view, rather than _intrinsically_ separating the universe into agent and outside. All else being equal, I prefer a representation which is continuous over the grand universe and marks no special boundary where the observer is located; as opposed to a representation which solidifies the Cartesian boundary between an observer-decider homunculus and the environment.

But as I said, you don't feel the Cartesian boundary in practice when working with explicit models, since the model boundary is so much tighter.

## Explicit models for Newcomblike problems

But what's fun about Newcomblike problems is you can get the decider in your little computable explicit model.
For example, [MIRI's modal agent prisoner's dilemma tournament](https://arxiv.org/abs/1401.5577).

To see the connection to Newcomb's problem, consider [David Lewis's retelling of the prisoner's dilemma](https://philpapers.org/rec/LEWPDI).
There's a thousand dollars in a little box, and a million dollars in a big box unless your opponent "defects" by taking their thousand.
If your opponent is a replica of yourself, then it's an instance of Newcomb's problem: taking both boxes gets you a thousand dollars more than taking just the big box regardless of its contents, but only those that leave the small box find a million in the big box.

In MIRI's dilemma tournament, the players are programs, with access to the other player's source code.
So not only do we have an explicit model of the decision problem, but we have an explicit model of the decider.
In fact, the decision problem they face is the other decider, and they are in Lewis's scenario when they face themselves.

The MIRI prisoner's dilemma tournament doesn't feel like a philosophy question, but more like a logic puzzle.
The program "decides", but only in the sense that a chess playing program decides on a move.

