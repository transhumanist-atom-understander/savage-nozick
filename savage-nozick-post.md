I'm a one boxer, but when I read the original Newcomb's problem paper and Nozick explained that you one-box to maximize expected value but two-boxing is the dominant solution, it sounded like nonsense to me.
Obviously a dominant solution is higher expected value, right?
If each possible result is higher utility, then they're higher utility on average.

What I want to communicate is not really why this is wrong, but why it would feel right.
In what I'll call "classical decision theory", for which my reference is Savage's book, dominance implies higher expected value.
I want to get you into my mindset where classical decision theory is not only correct but trivial.
This is worth doing because I think classical decision theory really does make sense, even physical sense, and helps more clearly see the essence of Newcomblike problems, which is embedding a description of the agent in the model.

I do think about this physically, because of my work in "virtual screening", in which we do quantum mechanical simulations of many molecules to decide which one to synthesize.
So for me, the model used for the decision problem is a physical model.
I think that how you can be satisfied with classical decision theory is the same as how you can be satisfied with Copenhagen quantum mechanics.
Which is: in science you work with explicit models.
When I simulate a molecule, in my computer I have a complete description of it: the atomic number and coordinates of each atom.
The kind of questions people ask in quantum interpretations, about a joint quantum state of the molecule and experimenter, don't feel natural.
Leaving aside how I don't know how to enter the experimenter in the simulation software, I don't even include an atom-level description of the solvent the molecule is in (at most using "implicit solvent", where we just change the dielectric constant).

Reading Savage's book, he seems to have the intellectual habits you develop from explicit modeling.
An interesting comparison between Savage and Nozick is how they use the term "state of the world".
It's important because I would say a dominant action is one that leads to a better result in every state of the world.
Savage explains that by "the world", he means "the object of interest".
For example, in the decision problem of what to do with an egg that may or may not be rotten, the world is the egg.
Readers concerned that this may be too narrow a conception of "the world" will find that he goes on to consider: "if the person is interested in the only brown egg in a dozen, should that egg or the whole dozen be taken as the world?"

Savage thinks of acts as maps from states of the world to consequences.
So those little tables we draw for decision problems look like:

$$\begin{array}
    & s_1      & s_2      \\
a_1 & a_1(s_1) & a_1(s_2) \\
a_2 & a_2(s_1) & a_2(s_2)
\end{array}$$

That $a_2$ dominates $a_1$ means that each consequence in the bottom row is preferred to the consequence directly above it.

Nozick also uses the term "state of the world", but I think what analytic philosophers mean by "the world" is really the "whole world".
I mean, why not, if you only talk in the abstract about descriptions of the world, and don't have the burden of actually writing one down and computing with it?
In the two by two table describing a decision problem, Savage sees two states of the world corresponding to the columns.
But Nozick sees four, since we are part of the world too.

The result is different conceptions of dominance.
As I said, in classical decision theory, dominance and expected value _can't_ conflict.
Let's go through that argument.
Let $p$ be the probability of $s_1$ and $q$ be the probability of $s_2$.
Let $U$ be the utility function (mapping consequences to numbers).
Let $U_1 = U \circ a_1$ be the utility resulting from act $a_1$, and likewise for $U_2$.
How much higher is the expected value of $U_2$ than $U_1$?

$$p U_2(s_1) + q U_1(s_2) - (p U_2(s_1) + q U_2(s_2) \\
= p (U_2 (s_1) - U_1(s_1)) + q (U_2(s_2) - U_1(s_2))$$

If $a_2$ dominates, both these terms are positive, so $U_2$ has higher expected value.

The "mistake", at least in a Newcomblike problem, was using the same probabilities when calculating the expectation of $U_1$ as $U_2$.
But for considering what to do with a rotten egg, this is fine.
And in my experience with virtual screening, it's extraneous even to consider multiple states.

For Nozick that sees four states in this table, the division into two columns is arbitrary, and he has a fun section where he reframes the problem to shuffle the table.
He defines dominance as relative to a "partition" of the states of the world.
That is, a partition of what Savage would consider (act, state) pairs.
And the above argument that dominance implies higher expected utility doesn't go through when we use probabilities conditional on acts.

What I'm hoping to communicate is the mindset where a joint distribution of states and acts is as foreign as a quantum state of an experimenter and a molecule.
They're the same thing really: something I can't enter into my quantum chemistry software, which I would consider unserious if I ever got around to considering it, which I don't, because I didn't even get as far as including the solvent in my model.
