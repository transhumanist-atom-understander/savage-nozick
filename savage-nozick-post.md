# Newcomb's problem from the grand-system and petty-system views

## A digression: the boundary around a quantum system

It's pretty easy to do quantum mechanics every day and never think about interpretations.
For example, using quantum chemistry software.
You input a molecule as a file with a row for each atom, each row containing the atom's element identity and xyz coordinates.
Just the atoms in the molecule and not the atoms in its surroundings, as if the molecule is floating in outer space, is enough for gas phase properties.

You can do some impressive calculations with modern software.
Erwin Schrödinger could calculate the hydrogen atom spectrum, but with a computer you can compute which frequencies of light will be absorbed by organic pigments used to dye clothes or as food colorings.
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

Similarly, I think you could use classical decision theory every day and never wonder about the critical issue in Newcomb's problem: the dependence of the state of the world on the person deciding.

My reference for what I'm calling "classical decision theory" is [Savage's book](https://archive.org/details/foundationsofsta0000sava/page/n1/mode/1up).
And as philosophical as that book is, it only makes sense to me when I read it from the perspective I've developed for explicit modeling.

In Savage's theory, an "act" is a function mapping a state of the world to a consequence.
Savage explains that by "the world", he means "the object of interest".
For example, in the decision problem of what to do with an egg that may or may not be rotten, the world is the egg.
Readers concerned that this may be too narrow a conception of "the world" will find that he goes on to consider: "if the person is interested in the only brown egg in a dozen, should that egg or the whole dozen be taken as the world?"

In [Nozick's paper introducing Newcomb's problem](https://philpapers.org/rec/NOZNPA), he thinks the world really means the whole world, which creates some interesting miscommunications with the classical theory.
What Nozick calls a "state of the world" is in Savage's theory a (state, act) pair.
This makes sense if you consider "the world" to include yourself.

What if you try to analyze Newcomb's problem without including yourself in "the world"?
Then the states of the world are simply "money in one box" and "money in both boxes", and all that classical decision theory tells you is that the act "take both boxes" maps both states to more money than the act "take one box".

Although this gives what I think is the wrong answer (two boxing), I think it's the right way to apply classical decision theory (either that, or just say Newcomb's problem is out of scope).
That we can have two different acts, mapping the same state to two different consequences, seems to require that this "state of the world" does not specify an act, and therefore that "the world" does not contain the actor.

But I don't think Savage even realizes that his formalism requires leaving the actor out of the world.
After proposing the world of a dozen eggs, he does consider that the state of the world may be the "exact and entire past, present, and future history of the universe". He doesn't mention that the universe includes the actor. Instead, he says that the problem is that it is "vague", and:

> It may also be added that the use of modest little worlds, tailored to particular contexts, is often a simplification, the advantage of which is justified by a considerable body of mathematical experience with related ideas.

It's true that if you want to actually derive consequences from explicit models, then you're used to simplifying to the bare minimum.
Perhaps that makes it easy to miss that including yourself in the model introduces special problems, since for the sake of simplification you don't get anywhere near including that much.

## The appeal of the grand systems perspective

In [his original paper on what we now call the "many-worlds" interpretation](https://doi.org/10.1103/RevModPhys.29.454), Everett motivated it with quantum cosmology, since there's nowhere outside the universe for a Copenhagen-style observer to stand.
[Eliezer Yudkowsky said something similar to motivate timeless decision theory](https://intelligence.org/files/TDT.pdf):

> I hold it a virtue of any decision theory that it should be compatible with a grand-system view, rather than _intrinsically_ separating the universe into agent and outside. All else being equal, I prefer a representation which is continuous over the grand universe and marks no special boundary where the observer is located; as opposed to a representation which solidifies the Cartesian boundary between an observer-decider homunculus and the environment.

But as I said, you don't feel the Cartesian boundary in practice when working with explicit models, since the model boundary is so much tighter.

## Explicit models for Newcomblike problems

But what's fun about Newcomblike problems is you can include the agent in your little explicit model.
For example, [MIRI's modal agent prisoner's dilemma tournament](https://arxiv.org/abs/1401.5577).

To see the connection to Newcomb's problem, consider [David Lewis's retelling of the prisoner's dilemma](https://philpapers.org/rec/LEWPDI).
There's a thousand dollars in a small box, and a million dollars in a big box unless your opponent "defects" by taking their thousand.

If your opponent is a replica of yourself, then the prisoner's dilemma becomes an instance of Newcomb's problem.
Taking both boxes gets you a thousand dollars more than taking just the big box regardless of its contents.
But the only players that find a million in the big box are those that didn't take the small box.
Any player taking both boxes finds that their replica has done the same thing, leaving them with only a thousand.

In MIRI's prisoner's dilemma tournament, the players are programs.
So not only do we have an explicit model of the decision problem, but we have an explicit model of the agent.

In fact, our model of the decision problem is really a model of another agent, the opponent.
And the trick is that your opponent has your source code to work with, which is how the money on the table can depend on which boxes you would take.
A program is in Lewis's scenario when it plays against another player defined by the same program.

The MIRI prisoner's dilemma tournament doesn't feel like a philosophy question, but more like a logic puzzle.
The program "decides", but only in the sense that a chess playing program decides on a move.
It's tricky due to the self-reference, but we can handle it with concepts from computer science and metamathematics.

If we want to use programs like these as models for situations involving ourselves, then we may run into familiar philosophical debates about whether we can think of our actions as the results of an algorithm.

But I guess it's important to me to have the philosophically boring, uninterpreted logic puzzle available.
It fits into a familiar scheme of scientific modeling.
We reason through explicit models with unambiguous implications, and with experience and taste that can help us understand the real world.
