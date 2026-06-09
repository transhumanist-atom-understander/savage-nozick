It's pretty easy to do quantum mechanics every day never think about interpretations.

I think it will help if I tell you about calculation that modern software can do, which I think is pretty impressive.
Given a molecular structure, what is its color?
<!-- Can cite this -->
Quantum chemistry can get pretty good predictions of the absorption wavelengths of real dye molecules.
The input is a file where each row is the element and xyz coordinates of an atom.
This represents the molecule floating in empty space.
The real measurements are in a solvent, but this is usually handled as an "implicit solvent", meaning we don't include the solvent atoms in the file, jut appropriately adjust the dielectric constant.

So suppose you're used to working with explicit atom-by-atom models, and think of quantum mechanics as a program that operates on such models, and then you consider perhaps the basic question in interpretations: after a measurement, what's the joint quantum state of the measured atom and the experimenter?
It's more than just that you don't have an atom by atom description of the experimenter, more than just that this is way too many atoms for the software to handle.
Yeah, I don't usually consider the experimenter, or the measurement device, but I also don't have a sense that I'm specifically leaving them out.
I mean, i don't even include the solvent.

I think you can also use what I'll call "classical decision theory", for which my reference is Savage, and never worry about Newcomb's problem, for similar reasons.
Savage's book only makes sense to me when I read it from the perspective I've developed in explicit modeling.
In his theory, an "act" is a map from a state of the world to a consequence.
Savage explains that by "the world", he means "the object of interest".
For example, in the decision problem of what to do with an egg that may or may not be rotten, the world is the egg.
Readers concerned that this may be too narrow a conception of "the world" will find that he goes on to consider: "if the person is interested in the only brown egg in a dozen, should that egg or the whole dozen be taken as the world?"

In Nozick's paper introducing Newcomb's problem, he thinks the world really means the whole world, which creates some interesting miscommunications with the classical theory.
What Nozick calls a "state of the world" is in Savage's theory a (state, act) pair.
This makes sense if you consider "the world" to include yourself.

I don't think Savage even realizes that his formalism requires leaving the decider out of the world.
After the dozen eggs, he does consider that the state of the world may be the "exact and entire past, present, and future history of the universe", but his objection to this is that it is "vague", and:

> It may also be added that the use of modest little worlds, tailored to particular contexts, is often a simplification, the advantage of which is justified by a considerable body of mathematical experience with related ideas.

It's true that if you want to actually derive consequences from explicit models, and not just say "consider some description of the whole world" without writing one down, then you're used to simplifying to the bare minimum.
Perhaps that makes it easy to miss that including yourself in the model introduces special problems, since for the sake of simplification you don't get anywhere near including that much.

<!-- Can do better on the EY and Everett qquotes -->
In quantum mechanics, Everett addresses "the quantum mechanics that is internal to an isolated system", and in decision theory, Yudkowsky wants to consider a "naturalistic" as opposed to "Cartesian" model.

In my work in "virtual screening", for which I do quantum mechanical simulations of many molecules to decide which one to synthesize, the model used for the decision problem is a quantum mechanical model.

Savage thinks of acts as maps from states of the world to consequences.
