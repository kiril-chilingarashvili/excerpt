---
layout: page
title: Bernoulli's Fallacy, Chapter 1 Excerpt
publish: false
---

# 1 

## WHAT IS PROBABILITY?


#### Abstract

Some of the Problems about Chance having a great appearance of Simplicity, the Mind is easily drawn into a belief, that their Solution may be attained by the mere Strength of natural good Sense; which generally proving otherwise, and the Mistakes occasioned thereby being not unfrequent, 'tis presumed that a Book of this Kind, which teaches to distinguish Truth from what seems so nearly to resemble it, will be looked upon as a help to good Reasoning.


Abraham de Moivre (1718)

Defining probability is more difficult than it might seem at first. Maybe you feel sure you already know what it is. If so, here's a warm-up exercise to make you less sure: Why is the probability of a coin flip coming up heads 50 percent? Maybe you answered that it's because, over a long series of flips, about half of them will come up heads - in which case here are two follow-up questions: (1) Have you ever actually flipped a coin enough times to convince yourself that what you think would happen will actually happen? (2) What about something like the weather forecast? Does the claim that there is a 30 percent chance of rain tomorrow mean that over a long series of tomorrows about 30 percent of them will be rainy? What about the probability that you'll live to be 100 or that the New York Mets will win the World Series? What about the probability that there is life on other planets?

Returning to the coin flips, maybe you said the answer is 50 percent because that's how sure you feel about the prospect of a coin coming up heads. What if your best friend said they were 99 percent sure a coin flip would come up heads
and wanted to bet their life savings on it? Would you try to talk them out of it? What if a casino offered you a million dollars to compute the right payoffs for a new video poker machine? Would you go by gut feel?

Or maybe you said it's because there are two possibilities and heads is one of them-ergo the chance is one out of two. Okay, so what's the probability the sun will rise tomorrow? Also 50 percent?

Or maybe you think the coin-flip probability is 50 percent because you have no information to prefer one outcome over the other, so you must assign them equal chances. How do you know what information you have? What would you say is the probability that the number $2^{2^{61}-1}-1$ is prime? Don't you think that, with the information you "have," you could eventually figure it out for sure?

If you find yourself feeling more confused the more you think about it, you're certainly not alone. Attempting to answer the question, What exactly do we mean by probability anyway? has frustrated mathematicians and philosophers for a long time, and as we'll see, that frustration has had ripple effects throughout scientific and statistical practice. To begin to get our heads around it, we'll start in ancient times and see how different people have tried to solve the puzzle of probability in various ways through the centuries and why their attempts were ultimately unsatisfying. That will bring us all the way back to the present day, where the question still isn't completely answered, but we can assemble the pieces we collect along the way into something that looks kind of like a start.

## THE CLASSICAL ANSWER

Advantages: Intuitive, works well for dice and card games.

Disadvantages: Doesn't work so well for anything else.

Ideas of fate, fortune, or luck and methods of generating chance outcomeseither for purposes of divination or just for fun - have existed in various cultures around the world since the beginning of recorded history. The Greeks had Tyche (called Fortuna by the Romans), the god of luck, whose responsibilities included safeguarding the city. The I Ching describes a method of fortune-telling in which the user gathers stalks of the yarrow plant, converts these to a number, and consults a corresponding prophetic hexagram. Ancient Egyptians played a dice game called Hounds and Jackals, and the Indus Valley civilization had a similar game, Gyan Chauper, which survives today in slightly modified form as Chutes and Ladders. The Romans had their aleae, rudimentary tetrahedral dice made
from the ankle bones of sheep, as memorialized in Julius Caesar's declaration upon crossing the Rubicon: "Alea iacta est." (The die is cast.) The Jewish holiday Purim (from the Akkadian pur meaning "fate") celebrates the story of the book of Esther, in which the Jewish people were saved from genocide on a date that had been chosen randomly. The biblical book of Leviticus refers to the high priest casting lots (in Hebrew, goralot) to decide the fate of a sacrificial goat or make other priestly decisions, and the Gospels also describe Roman soldiers casting lots (in Greek, kleron meaning "portion") to see who would get Christ's cloak after the Crucifixion.

Our word probability, from the Latin root probare meaning "to test," is therefore related to several other English words involving testing, including probe, proof, approve, and probity. The connection between probability and relative soundness or believability was present from the earliest times. Aristotle's Rhetoric described "the Probable" (in Greek, eikos, from eoika meaning "to seem") as "that which happens generally but not invariably." The context for this was his classification of the arguments one could use in a courtroom or legislative debate, where perfect logical deductions may not be available. He called this form of argument an enthymeme, to be distinguished from the purely logical form of argument called the syllogism, which links together a set of assumed premises to reach deductive conclusions, as in this famous example:

All men are mortal.

Socrates is a man.

$\therefore$ Socrates is mortal.

Often, Aristotle observed, pure logic won't suffice on its own because some links in the chain are missing or uncertain. But he offered the advice that "we should also base our arguments upon probabilities as well as upon certainties,"2 and this could still constitute an appeal to good reason, since "the true and the approximately true are apprehended by the same faculty; it may also be noted that men have a sufficient natural instinct for what is true, and usually do arrive at the truth. Hence the man who makes a good guess at truth is likely to make a good guess at probabilities."3

A standard of ancient and medieval legal proceedings was that testimony or evidence, even if not providing absolute certainty, could be (in Latin) probabilis meaning "credible and generally agreed upon." The Talmud even suggested that some doubt was a necessary component of justice because a feeling of absolute
certainty meant a judge had not properly examined all the arguments to find the holes in them. In a capital case before the lesser Sanhedrin, the rule was that if all 23 judges voted to convict, then the suspect was acquitted. Probable opinions were those we humans hold to be true within the limits of our own fallible judgment. It was in this sense that Cicero, writing about the nature of the gods, advised that probability "should guide the life of a wise person."4

In ancient times, chance was purely qualitative, likely for two main reasons: (1) arithmetic was still carried out mostly using Roman numerals, which made probability calculations awkwardly difficult, and (2) the only things people had to gamble with were sheep ankle bones and other unpredictably shaped objects, which didn't behave reliably enough to bother with numerical probabilities. But by the Renaissance, when gaming equipment was more reliably crafted and real money was on the line, the mathematics of chance started to become a topic of concern. What should be the fair odds for a bet on a dice or card game? Even educated people found they were unable to answer the basic questions that naturally presented themselves.

The French gambler Antoine Gombaud, who gave himself the nickname of Chevalier de Méré, had a particular interest in what became known as the problem of points. Here's the basic setup:

You and I are playing a game with equal chances of winning each round (such as flipping a fair coin), with the result that each time I win I earn 1 point and each time you win you earn 1 point. We start at $0-0$ and play until one of us gets to some number of points, say 5 . The winner gets $\$ 100$. However, suppose at some intermediate point, say with you leading by a score of $3-1$, the game is interrupted. How should we divide up the stakes?

On the one hand, it seems unfair to you if we simply call off the game and divide the stakes equally. After all, you are significantly ahead and well on your way to victory. On the other hand, it seems unfair to me if I'm made to forfeit entirely; it's still possible I could come back to win. So what should we do? Various gamblers had encountered this problem and attempted a fair division of the stakes by different means but without a clear mathematical reason to justify the division.

Gombaud posed this question to his friend, the mathematician and philosopher Blaise Pascal, who in 1654 was able to work out a rigorous solution in a series of letters with fellow member of the Académie Parisienne and mathematical superstar Pierre de Fermat. In the process, the two of them effectively created probability theory. The main idea of their solution was to divide the
stakes according to what we would now refer to as each player's expected value. That is, we could imagine playing the game out to its conclusion (considering each of the remaining sequences of wins and losses to be equally likely), tally up the scenarios in which each player won the full prize, and finally divide up the stakes according to how many scenarios led to a victory for each player. In modern language, we would say the outcomes (you win) and (I win) were given a probability distribution, and the weighted average payoffs were given to each of us as a fair value of our position in the game.

The word chance, from the Latin cadentia meaning "a case, an instance," thus had something of a legal connotation. An event or claim was deemed to be probable or likely according to the number of "cases" for it, as though each possible outcome were an argument or piece of evidence in a courtroom. A fair judgment for an uncertain claim was the one given according to the weight of evidence in favor of each claimant. Fermat, in particular, would have found this way of thinking familiar, since he was previously a lawyer and magistrate of the court at Toulouse. The legal analogy, within an all-encompassing view that probability should apply to all reasoning, was apparently on Jacob Bernoulli's mind when he wrote Ars Conjectandi, which includes multiple suggestions for the application of probability to legal decision-making. He began chapter 2 of book IV with this preamble discussion:

The art of conjecturing or stochastics is defined as the art of measuring the probability of things as exactly as possible, to be able always to choose what will be found the best, the more satisfactory, serene and reasonable for our judgements and actions. This alone supports all the wisdom of the philosopher and the prudence of the politician. Probabilities are estimated both by the number and the weight of the arguments which somehow prove or indicate that a certain thing is, was, or will be. As to the weight, I understand it to be the force of the proof. ${ }^{5}$

He then considered the many different forms of argument that might be presented in an example of a suspect accused of murder:

Titius is found killed in the street. Maevius is charged with murder. The accusing arguments are: 1) He is known to have hated Titius (an argument from a cause, since this very hate could have incited to murder. 2) When questioned, he turned pale and answered timidly (this is an argument from the effect since it is possible that the pallor and fright were caused by his being conscious of
the evil deed perpetrated). 3) Blood-stained cold steel is found in Maevius' house (this is an indication). 4) The same day that Titius was killed, Maevius had been walking the same road (this is circumstance of place and time). 5) Finally, Cajus maintains that the day before Titius was killed, he had quarrelled with Maevius (this is a testimony). ${ }^{6}$

For these reasons, the theory of probability in the beginning days was known as the doctrine of chances-most prominently in the title of French mathematician Abraham de Moivre's seminal textbook on the subject, The Doctrine of Chances: Or, a Method of Calculating the Probability of Events in Play (published in 1718). The conventional definition of probability was what we would now call the "classical" one:

$$
P[\text { event } A]=\frac{\# \text { ways event } A \text { can occur }}{\# \text { possible outcomes that can occur }}
$$

In fact, this persists as the definition given in most introductory probability textbooks today.

The main calculation required to solve any probability problem under the classical definition, then as now, was counting the possibilities for the numerator and denominator of this fraction. Pascal, in particular, was helped by the triangle that now bears his name, tabulating the number of combinations of any $n$ objects taken $r$ at a time, which is a regular ingredient for such computations. For example, if we were computing the probability of getting three heads in a sequence of five coin flips, we might at some point need to know how many such sequences there are, depending on the order in which the flips occur. Pascal's formula gives us the answer:

$$
\left(\begin{array}{l}
5 \\
3
\end{array}\right)=\frac{5 !}{3 !(5-3) !}=10
$$

However, a subtle difficulty arose in some problems where the accounting of possible outcomes was not so clearly apparent. For example, around 1620 Ferdinando dei Medici, the Grand Duke of Tuscany, became bothered by a particularly thorny problem of dice probabilities and sought help from a beneficiary of his patronage, who, luckily for the duke, was Galileo Galilei. The problem was to determine whether 9 or 10 was more probable as a sum of three six-sided dice. It seemed from one way of counting that they were equally likely,
since each could be written as a sum in six distinct ways (ordering the terms from greatest to least):

$$
\begin{gathered}
9=6+2+1=5+2+2=5+3+1=4+3+2=4+4+1=3+3+3 \\
10=6+2+2=6+3+1=5+3+2=5+4+1=4+3+3=4+4+2
\end{gathered}
$$

The duke, who was both a compulsive gambler and an extremely observant person, had noticed 10 seemed to come up slightly more often but was at a loss to explain why. Galileo's insight was that counting outcomes according to the numbers they contained was the wrong way of counting. Instead, he argued, one should keep track of which die produced which number. Imagining the dice to be colored red, white, and green, he showed that, for example, the combination $(3,3,3)$ could be found only one way, with all dice turning up 3 , while the combination $(6,2,1)$ could occur six different ways, depending on the permutation of colors. Combinations such as $(5,2,2)$ could likewise show up in any one of three different configurations of dice. Thus, in the final tally there were 25 possible ways to get a 9 and 27 to get a 10 out of the 216 possible rolls, making 10 ever so slightly more probable.

So even a simple dice game could produce some confusion over the proper way to do the counting. This issue continues to confuse students of probability to the present day. Many struggle with problems like this one:

You and two of your friends are in a group of 10 people. The group is randomly split up into two groups of 5 people each. What is the probability you and both of your friends are in the same group?

Solutions may involve distinctions like whether the groups are "labeled" or "unlabeled" and so on.

The implicit understanding present in the classical definition of probability was that the enumeration of outcomes must be done in such a way that they are equiprobable, or equally likely to occur. These are the tiny atoms from which all probabilities are then built. But, of course, this couldn't be an explicit requirement because then the definition would be circular: probability depends on probability. Most current authors attempt to dodge this by saying the outcomes must be equally "likely," but what is likelihood if not probability?

For most simple problems, the enumeration of equally likely cases was selfevident because of some apparent symmetry-the six faces of a die all seem roughly the same, for example. But what about lopsided or misshapen dice?

Unless chance was measurable some other way, there would always be some doubt the counting had been done properly. Furthermore, some problems to which we'd like to apply probability, such as forecasting tomorrow's weather or determining the guilt of a murder suspect, seem resistant to this kind of description at all. If we claim a 5 percent chance there will be a major earthquake in the next year, what are the equiprobable outcomes out of which 5 percent involve an earthquake and 95 percent don't? Attempts to imagine some theoretical population of equally likely worlds out of which ours is randomly drawn seem forced, at best. Despite the success of the classical interpretation for simple games of chance, there was an apparent need for a new, more experimentally verifiable approach to defining probabilities.

## THE FREQUENTIST INTERPRETATION

Advantages: Empirically testable.

Disadvantages: Doesn't work for rare events, one-time events, or past events.

It was clear from the Duke of Tuscany's analysis of his dice problem that some connection was assumed between the probabilities of events and their occurrences in repeated observation - that is, their relative frequencies. The grounding of probability in observable fact was even already present in Aristotle's definition of the probable as "that which happens generally." Insisting probabilities numerically match empirical frequencies seemed to resolve any question about whether the decomposition of outcomes into equiprobable atoms had been done correctly, at least when the frequencies were known or knowable.

Enter Bernoulli's Law of Large Numbers, which he called his "golden theorem." Bernoulli imagined a situation where the number of cases for and the number of cases against some outcome, like the number of possible dice rolls with a given sum, were unknown. He then asked what could be expected to happen over a large number of observations. What he was able to show was that the observed frequencies would necessarily converge to the true probability as the number of trials got larger. Consider, for example, a game where a friend is rolling three dice and telling us the total, but we don't know whether they're 6-, 8-, or 12-sided dice or whether they're numbered in the usual way. We want to know the probability of getting a 10 . We could try to figure it out by asking to inspect the dice and working out all the possible sums with their
associated probabilities for ourselves, or we could just allow our friend to roll the dice a large number of times and tally up how often 10 shows up. According to Bernoulli, if the number of trials is sufficiently large-say a few million or billion - these two procedures will almost certainly give approximately the same answers.

His claim was that by establishing this convergence of frequencies to probabilities, he had provided a means of determining, to within a small error and with some "moral certainty," an unknown probability: "If, however, this is attained and we thus finally obtain moral certainty . . . then we determine the number of cases a posteriori [after doing the sample] almost as though it was known to us a priori [before doing the sample]."7

Bernoulli didn't confine himself to games of chance, though. In the opening of chapter 4 in part IV of Ars Conjectandi, he gave an example of determining a person's chance of living 10 more years by tallying up the results of men of the "same age and complexion":

It should be assumed that each phenomenon can occur and not occur in the same number of cases in which, under similar circumstances, it was previously observed to happen and not to happen. Actually, if, for example, it was formerly noted that, from among the observed three hundred men of the same age and complexion as Titius now is and has, two hundred died after ten years with the others still remaining alive, we may conclude with sufficient confidence that Titius also has twice as many cases for paying his debt to nature during the next ten years than for crossing this border. ${ }^{8}$

Here, "number of cases" meant the factors determining the true probability, as in the numbers of black and white pebbles in an urn, even if those weren't countable in any other way. So a sample of 300 men would give us "sufficient confidence" to conclude the real mortality rate was the same as what we had observed. To Bernoulli, this was self-evidently the correct way to determine probabilities in all manner of different settings, from simple experiments involving urn drawing to real-world problems dealing with mortality, incidence rates of disease, occurrence of weather events, and even guilt or innocence of defendants in trials.

This all may seem obvious now, but before Bernoulli, there was no mathematical guarantee that frequencies had to match probabilities; it just felt intuitively right. He saw his main contribution, the Law of Large Numbers, as justifying this intuition. Without something like Bernoulli's theorem, how could we really
know our observed frequencies wouldn't converge to some value other than the true single-event probability? For example, what if the real probability of rolling a double-six with two dice is $1 / 36$, but over the long run, the frequency we actually observe stabilizes at $1 / 35$ or $1 / 37$ ? Bernoulli put this concern to rest.

In the centuries following Bernoulli, as empiricism began to crescendo, some made the leap to claiming this long-run frequency of occurrence was actually what the probability was by definition. Bernoulli had opened the door to this way of thinking by including examples like those above, where establishing probability was not possible except by measuring frequency. How else, for example, could you come up with the "number of cases" for and against Titius living another 10 years except by observing how often similar people lived that long? If the frequency is the only available means of calculating the probability, it may as well serve as the definition. As we'll see later, this interpretation especially gained traction after probability took hold in social science; in the mid19th century, John Stuart Mill, Robert Leslie Ellis, Antoine Augustin Cournot, Jakob Friedrich Fries, and the logician George Boole all described probabilities in terms of frequencies of occurrence.

Perhaps the greatest proponent of the frequentist view was the English logician and philosopher John Venn (of Venn diagram fame). He came from a family with a long tradition of being ordained clergy, and after studying mathematics at Cambridge, he briefly joined the family business as an Anglican priest before returning to Cambridge to teach morality, logic, and probability theory. Reflecting his time in the pulpit, his mathematical writing often reads more like a sermon than a math paper. In his groundbreaking book The Logic of Chance (1866), Venn lamented that probability had not received the rigorous treatment he thought it deserved and only philosophers could provide:

Probability has been very much abandoned to mathematicians, who as mathematicians have generally been unwilling to treat it thoroughly. They have worked out its results, it is true, with wonderful acuteness, and the greatest ingenuity has been shown in solving various problems that arose, and deducing subordinate rules. And this was all that they could in fairness be expected to do. . . But from this province the real principles of the science have generally been excluded, or so meagrely discussed that they had better been omitted altogether. ${ }^{9}$

He then attempted to formalize the frequency interpretation of probability and iron out some of the practical difficulties of applying this definition that had tripped up previous authors.

For example, taking the frequentist view, we may say the chance of a coin flip coming up heads is the relative frequency of heads in a long series of repeated coin tosses. But how long is "long"? In any finite sequence of coin flips, the proportions of heads and tails will always add up to 100 percent, but we could expect some variation around the true "long-term" answer. The whole point of Bernoulli's theorem was to show that the variation probably wouldn't be too much, but it would still be present. We wouldn't say the probability of heads was 50.1 percent just because we saw 501 heads out of 1,000. Venn argued we need to consider the limit as the number of trials goes to infinity. That limiting frequency is the precise probability of the event.

However, this, of course, presents a practical impossibility: we can't flip a coin an infinite number of times. Furthermore, even flipping a real coin a very large number of times introduces with near certainty the fact that the characteristics of the coin will change over time-it will gradually get dented, scratched up, or bent out of shape. Venn's answer was that one should imagine repeating the infinite series of trials with no change to the relevant underlying factors. That is, we should imagine flipping an imaginary coin. Yet somehow the results of this are still held to be materially meaningful and, according to Venn, the only acceptable definition of probability.

In fact, Venn went so far down the frequentist rabbit hole he even left Bernoulli's Law of Large Numbers behind. Bernoulli, drawing on the classical interpretation, had described an experiment as having a "true probability" for a single event and had derived the probability of an observed sample falling within some bounds of that true value. However, for Venn and others who were trying to extend the reach of probability beyond the classical interpretation, there was no such thing as the "true probability" in any sense other than the long-run frequency of occurrence. From Venn's point of view, the Law of Large Numbers was tautological; it was trivial to claim the long-run frequency of an event's occurrence would converge to the probability if the frequency was taken to be equal to the probability by definition. Concerning Bernoulli's theorem, Venn wrote, "With the mathematical proof of this theorem we need not trouble ourselves, as it lies outside the province of this work; but ... the basis on which the mathematics rest is faulty, owing to there being really nothing which we can with propriety call an objective probability."10

The French mathematician Pierre-Simon Laplace (whom we'll be hearing more from later on) had once written that when we look at nature, we begin to detect "a striking regularity which seems to suggest a design, and which some have considered a proof of Providence. But, on reflection, it is soon perceived
that this regularity is nothing but the development of the respective probabilities of simple events, which ought to occur more frequently as they are more probable."1 Venn dismissed this as pure nonsense, calling Laplace's statement "a somewhat pretentious re-statement of the fact already asserted,"12 since for Venn there was no meaning to the probabilities of events other than how often they occurred.

Venn's dogmatic view of probability caught on in the sciences. In particular, it profoundly influenced the methods developed by the statistician Ronald Fisher, who may have been directly exposed to Venn's ideas while an undergraduate at Gonville and Caius College, Cambridge, when Venn was the college president. In his book Statistical Methods and Scientific Inference (1956), Fisher laid out what he understood to be the correct definition of probability, and he credited Venn with "developing the concept of probability as an objective fact, verifiable by observations of frequency."13 We'll be coming back to Fisher and frequentist statistics.

Some technical issues with the frequentist interpretation continued to be an annoyance well into the 20th century. For example, Venn's definition presupposes that the limiting frequency actually exists, which means mathematically it's important to consider exactly what kinds of sequences we are dealing with when we talk about random trials and in what manner this convergence takes place. The requirement simply that an infinite series of coin flips have limiting frequency $1 / 2$ would be satisfied if the coin flips came out to be HTHTHTHTHTHTHT ... with the pattern repeating forever, but that's clearly not the kind of sequence we should expect from a real coin. It's not "random" enough. But how to make randomness (from the old Germanic root rinnana meaning "run") precise while assuming the long-run frequency is known turns out to be harder than you might think. Venn said a truly random series with a given limiting frequency should exhibit "an order, gradually emerging out of disorder" 14 but didn't try to express this in any more exact way.

Around 1919, the Austrian mathematician Richard von Mises made a valiant effort. He defined a random sequence, which he called a Kollektiv, as having the property that we can't select any of its members to produce a subset with a frequency different from the overall limit. So, in the above example, if we picked out every other coin flip, we'd have a sequence of all heads or all tails, and these would have frequency 1 or 0 , not 1/2. A truly "mixed-up" sequence should be immune to having the heads or tails results selected according to any pattern or rule.

Unfortunately, in a purely mathematical sense this doesn't quite work because we can just define the selection rule to be "select an element of the sequence
if and only if the outcome is heads." Even though it seems like cheating, that's an allowable function according to the set-theoretic axioms of math, so no random sequence meeting such a broad criterion could ever exist. To get around this problem, von Mises tried for a while to restrict the kinds of rules we can use to select sequence terms, but in the end, he wasn't able to formalize them in a satisfactory way.

In 1940, the American mathematician Alonzo Church took up the charge, applying some of the then brand-new concepts of theoretical computer science. His idea was that the selection rule should be computable, meaning the decision to include a particular sequence term should be the result of some computer program applied to the previous part of the sequence as the "input data." Since there are only so many possible programs, he was able to show this did, in fact, allow for the existence of truly random sequences.

One final wrinkle, though, is that it turns out there are still sequences satisfying even this restrictive definition yet without the properties we'd want from true randomness. For example, the French mathematician Jean Ville observed in 1939 that, with respect to any countable collection of selection rules (which Church's computer programs were), there would always exist a sequence of heads and tails results with limiting frequency $1 / 2$ satisfying the selection-rule requirement, but with the weird property that if you stopped the sequence at any finite point, ${ }^{15}$ the proportion of heads would always be greater than or equal to $1 / 2$. So, over the lifetime of any finite number of coin flips, wed always have at least as many heads as tails. That, again, just doesn't feel right. For real coin flips, we'd expect the running total number of heads to be sometimes more and sometimes less than the number of tails and the proportions to oscillate above and below $1 / 2$ on the way to stabilizing. But Church's formal definition of randomness couldn't guarantee that would happen, and the problem of replacing it with a more satisfying definition is, in fact, still open.

Putting these theoretical issues aside, though, the frequentist interpretation of probability offers an appealing degree of objectivity, which likely explains its popularity among scientists. Instead of worrying forever about whether we have enumerated all the possible equally likely cases and counted up the ones corresponding to some event of interest, we can rest assured that, in principle, we can always verify probabilities (at least approximately) by conducting experiments. This puts probability on the same footing as other measurable quantities of physical systems like mass, density, and specific heat. Even though a single measurement may have some embedded error, over enough repeated observations we can narrow in on the true theoretical value or at least rule out values too far outside our observed range.

Combining noisy observations of a particular quantity — say the position of a planet in the night sky - had been a practical problem facing astronomers and physicists for a long time, and the technique of averaging measurements was known as a good practice since antiquity. So, if averaging noisy measurements of a physical quantity seemed to produce reliable estimates of the true value, then averaging the observed number of occurrences of an event-that is, calculating its observed frequency - seemed a natural way to estimate the true probability of the event each time. Bernoulli's theorem seemed to back this up mathematically.

But the cracks in the frequentist interpretation begin to show when even a little pressure is applied. For example, consider the frequentist answer to the question of the probability of an extremely rare event. If asked for, say, the probability of being dealt all 13 spades in a hand of bridge, any well-trained frequentist would no doubt begin with the calculation $(13 / 52) \cdot(12 / 51) \cdot(11 / 50) \cdot \ldots \cdot(1 / 40)$, reasoning there are 13 spades out of 52 cards available for the first card dealt, 12 spades out of 51 cards remaining for the second card, and so on. The frequentist would then ultimately arrive (hopefully with the aid of a computer) at the extremely small probability of 1 in 635,013,559,600.

However, there is no empirical evidence for this value as the limiting frequency of the event, nor will there ever be, since this is several orders of magnitude greater than the number of bridge hands ever dealt. Assuming we could deal one complete hand per minute and record the results, to get through one cycle of over 635 billion hands would require 1.2 million years. And, remember, in all that time our expected number of occurrences of the all-spades hand in question would be one! What if we saw two or none? Presumably, to establish the above probability as correct with any accuracy, we would need many more observations, taking perhaps billions or trillions of years.

Even that may not satisfy the frequentist. Imagine that after our impossibly long process of shuffling and dealing out trillions of bridge hands was complete, we arrived at a different limiting frequency than the one predicted-say we got something like twice as many perfect all-spades hands as expected. In that case, the frequentist would certainly claim something had gone wrong with the shuffling and dealing of the cards, so they were not truly "randomized" or had not been independent of one another! So there's an inherent circularity in the definition of probability in terms of frequency: the probability is the frequency we would get-but only if the conditions of the experiment were managed correctly, which we could discern only by the frequency coming out to be nearly equal to the probability.

Evidently even the adherents of this definition do not hold to it strictly in practice, since even in simple thought experiments like this one, they are able to
compute probabilities with absolutely no basis in empirical frequencies, relying on rules of calculation from somewhere that are so strong they would trump the frequencies even if they had been observed. Where do these principles come from, and how are they justified? We'll return to this point later on when we discuss Edwin Jaynes's view of probability and logic.

Where the frequentist interpretation struggles most, though, is in handling probabilities of one-time events. For example, if we want to say a certain politician has a 29 percent probability of winning the next election, how can this statement even be given a meaning in terms of frequencies? The election will happen only once, and even if we could imagine repeating it, à la Venn's imaginary coin flips, what conditions would have to change each time in order to produce different outcomes at all? If the election were held again, wouldn't all the voters vote the same way?

The question of what exactly counts as an independent trial and what characteristics these trials need to share becomes especially complicated when applying the frequency model to social science. It's easy to recognize a legitimate trial of a coin toss when we see one, but what if we wanted to estimate, say, the probability that a given person will live to be 90 , as an actuary would need to do for a mortality table? In principle, the frequentist interpretation would tell us to estimate this probability by finding a large collection of similar people-as in Bernoullis "same age and complexion" requirement-and counting the proportion among them who live past 90 . But similar in exactly what ways? The more identifying characteristics we include-male, age 40, nonsmoker, overweight, family history of diabetes, etc. - the smaller the reference class becomes until we're necessarily left with only the one person with whom we started. So are these probabilities only ever 0 or 1 ?

Too large a reference class would also pose a problem because it might give us accurate estimates of frequency that are practically useless. For example, here is a way to give very accurate weather forecasts for, say, the chance of rain in your local area without any meteorological training or equipment: simply look up the long-run historical frequency of rain for that area, and give this number as your predicted chance of rain every day. After a few years or so have gone by, the observed frequency will closely match your prediction, assuming the climate on the whole continues roughly as it was. But from day to day, your predictions won't incorporate any new information that would actually be useful for people trying to decide whether they need to bring an umbrella that day.

Venn had actually raised this issue of what should count as a trial for estimating a given probability, which later became known as the reference class
problem, in The Logic of Chance: "Every individual thing or event has an indefinite number of properties or attributes observable in it, and might therefore be considered as belonging to an indefinite number of different classes of things. ${ }^{\text {" }} 6$ But he failed to provide a satisfying answer, as has every other frequentist since.

Similarly, we can't apply a frequentist interpretation to events in the past because the frequency model allows only for contingent future outcomes we would observe if we conducted a series of experiments. So there is no (nontrivial) frequentist answer to questions like these: What is the probability that the mass extinction at the end of the Cretaceous period was caused by a comet? What is the probability that Shakespeare's plays were written by Francis Bacon? Such questions require a version of probability suitable for inference, which the frequentist interpretation simply can't easily handle.

## THE SUBJECTIVE INTERPRETATION

Advantages: Flexible, applies everywhere.

Disadvantages: Flexible, applies nowhere.

During the later years of his life in the 1740s and '50s, Thomas Bayes, an English Presbyterian minister and amateur mathematician who had studied logic and philosophy at the University of Edinburgh, became greatly interested in the subject of probability. One possible explanation for his interest was that, around the same time, the Scottish philosopher David Hume argued in An Enquiry Concerning Human Understanding that valid conclusions about the world could not be arrived at through experience. Hume's general point, later referred to as the problem of induction, was that we have no way of knowing experience is a guide for valid conclusions about the future because if we did, that claim could be based only on past experience. In other words, we only think the future will be like the past because as a rule "The future will be like the past" has always worked in the past. This means the argument from experience is necessarily circular. In section 10, titled "Of Miracles," he directed particular criticism toward the idea of empirical evidence for miracles, arguing one should not rely on supposed eyewitness testimony of their existence, such as the accounts of the Resurrection given in the Gospels.

Bayes may have been particularly motivated for religious reasons to prove Hume wrong by providing an explicit counterexample of valid induction, which he attempted to do by addressing a problem raised by de Moivre some 30 years earlier.

The problem was one of probabilistic inference. To take a slightly simpler version of the example Bayes considered, imagine the following dice game:

Your friend rolls a six-sided die and secretly records the outcome; this number becomes the target $T$. You then put on a blindfold and roll the same sixsided die over and over. You're unable to see how it lands so, each time, your friend (under the watchful eye of a judge, to prevent any cheating) tells you only whether the number you just rolled was greater than, equal to, or less than $T$. After some number of rolls, say 10 , you must guess what the target was. What would be your strategy for guessing, and how confident would you be?

Probability textbooks like de Moivre's could give some of the probabilities needed for the answer but couldn't solve the whole thing. For example, suppose in one round of the game we had this sequence of outcomes, with G representing a greater roll, $\mathrm{L}$ a lesser roll, and $\mathrm{E}$ an equal roll:

$$
\text { G, G, L, E, L, L, L, E, G, L }
$$

If the target number is 3 , for instance, then we could say the probability of any given roll being greater than $T$ is $3 / 6$, or $1 / 2$ (corresponding to rolls of 4,5 , and 6), and the probability of being less than $T$ is $2 / 6$, or $1 / 3$ (corresponding to rolls of 1 and 2). The remaining probability of rolling an equal number is always 1/6. Applying the rule of multiplying probabilities for independent trials, we could say the probability of getting that particular sequence is

$$
\left(\frac{1}{2}\right)\left(\frac{1}{2}\right)\left(\frac{1}{3}\right)\left(\frac{1}{6}\right)\left(\frac{1}{3}\right)\left(\frac{1}{3}\right)\left(\frac{1}{3}\right)\left(\frac{1}{6}\right)\left(\frac{1}{2}\right)\left(\frac{1}{3}\right), \text { or } \frac{1}{69,984}
$$

But all that assumes the target value is 3 to begin with. Similar calculations could apply to other choices of $T$, but then what? The probability rules of Bernoulli, de Moivre, and company couldn't tell us how to assemble these numbers into an answer to the inverse question: What is the probability that $T=3$ given the observation?

To accomplish this, Bayes needed to prove an identity involving the conditional probabilities for any two events $A$ and $B$, an equation we now call Bayes' theorem:

$$
P[A \mid B]=P[A] \frac{P[B \mid A]}{P[B]}
$$

The probabilities with the vertical bars refer to conditional probabilitiesthat is, the probability of event $\mathrm{A}$ assuming event $\mathrm{B}$ has happened, and vice versa. So $A$ could represent a hypothesis, like our guess about the target number, and $B$ could represent our observation, the sequence of greater, lesser, and equal results we're given. With elegant simplicity, the rule tells us how the probability of $A$ given $B$, the quantity we want, is related to that of $B$ given $A$, the probability we already calculated. Thus, assuming we have the other necessary ingredients, we can use the equation to switch from one logical direction to the other. Amazingly, this little equation - and what it implies about the nature of scientific inference-has been the source of an immense amount of controversy spanning four centuries now. The remainder of this book will consist mostly of exploring that controversy, but it all starts here.

The identity was likely known before Bayes and becomes apparent if we think of probabilities as relative proportions. Suppose, for example, we're interested in two characteristics among a group of individuals-say whether someone is a clown $(A)$ and whether they wear big shoes $(B)$. Maybe we are given that 20 percent of the people in this group are clowns $(P[A]), 25$ percent of the people wear big shoes $(P[B])$, and 80 percent of the clowns wear big shoes $(P[B \mid A])$. Say we see someone wearing big shoes, and we'd like to know the chance that they're a clown $(P[A \mid B])$ - that is, we want the proportion of $B$ who are also $A$. The natural way to compute the ratio is to find out how many big-shoed clowns there are $(A$ and $B)$ and then divide by the total number of people with big shoes. Imagine the total population consists of 100 people. Then we are assuming 20 are clowns, of whom 80 percent—that is, 16 - are big-shoed clowns. As a proportion of the 25 people with big shoes, this intersection group makes up $16 / 25$, or 64 percent, so this is the conditional proportion of those with big shoes who are clowns. Bayes' theorem just shows these quantities relate the way we have reasoned here.

The main innovation of Bayes's solution, though, presented and clarified somewhat after his death by his friend and fellow minister Richard Price, was that this conditional probability idea would apply to events, no matter the order in which they occur in time. So, if we were interested in events $E_{1}$ and $E_{2}$, with $E_{1}$ necessarily having the chance to occur first, we could reason just as well about $P\left[E_{1} \mid E_{2}\right]$ as we could about $P\left[E_{2} \mid E_{1}\right]$, even though the latter seems more natural. This gave Bayes a tool to use for inverse problems, relating the "forward-looking" probabilities he could already compute to the "backwardlooking" ones he wanted to compute.

In our example problem involving the six-sided die, we would say conditionally on the observed data $D$ recording our sequence of greater, lesser, and equal outcomes, the probability of the target being 3 could be found by

$$
P[T=3 \mid D]=P[T=3] \frac{P[D \mid T=3]}{P[D]}
$$

We already handled the term $P[D \mid T=3]$ when we multiplied the probability fractions together and got 1/69,984. This is, as it usually will be, the easiest part, since it's the most "ordinary" probability calculation in the bunch; it represents the probability of getting a certain sequence of outcomes assuming a given setup. To finish the calculation, we have two missing pieces: $P[T=3]$ and $P[D]$, unconditional on any assumed target value. The first term, $P[T=3]$, represents our initial probability for the proposition $T=3$ before we make any observation. In this case, since the target was the result of the initial roll of the die, we would say $P[T=3]=1 / 6$. Similarly, we would give the same prior probability to $T=1, T=2$, etc.

The denominator term requires the most attention, but Bayes recommended a general strategy: break the probability down into the possible cases and sum them. That is, we know the target number must be one of the numbers $1, \ldots, 6$. For each possibility, we can carry out calculations similar to the previous one to get the conditional probabilities of the data assuming $T=1, T=2$, up to $T=6$. The rules of (ordinary, forward-looking) probability tell us the total probability for $D$ is then the sum

$$
P[D]=P[T=1] \cdot P[D \mid T=1]+\ldots+P[T=6] \cdot P[D \mid T=6]
$$

That is, $T$ could equal 1 (with the given probability) and wed observe $D$ with the conditional probability $P[D \mid T=1]$, or $T$ could be 2 and we'd observe $D$ with conditional probability $P[D \mid T=2]$, etc. Since these are mutually exclusive cases forming "pathways" to the data $D$, we add them up to get the total probability of observing $D$.

Our prior probabilities for the various target values were uniform with probability $1 / 6$ for each, as shown in figure 1.1.

But after applying Bayes's process for the various target values for the given observation $D$, we find the posterior probability assignments $P[T=t \mid D]$ are concentrated around $T=4$, as shown in figure 1.2.

![](https://cdn.mathpix.com/cropped/2023_12_26_1ff88ac1c4f9832c7bebg-20.jpg?height=544&width=978&top_left_y=270&top_left_x=270)

FIGURE 1.1

Prior probabilities for the target guessing game.

![](https://cdn.mathpix.com/cropped/2023_12_26_1ff88ac1c4f9832c7bebg-20.jpg?height=546&width=978&top_left_y=1193&top_left_x=270)

FIGURE 1.2

Posterior probabilities for the target guessing game using Bayes' theorem.

In fact, we are 50 percent confident $T=4$, with some possibility remaining that $T=3$ or $T=5$ and a very slim chance $T=2$. Note we have ruled out $T=1$ and $T=6$ completely. We could have accomplished this by deductive reasoning, since any observation of a "greater" roll rules out the target being 6 and any "lesser" roll rules out the target being 1 and we observed both. However, there's no need for us to make a special case out of these, since Bayes' theorem works perfectly well when the probability is 0 , meaning the data is impossible given a particular hypothesis. (We'll return to this point when we connect Bayes' theorem with deductive logic.)

This same process will apply to any problem of inference among multiple hypotheses. In fact, this will be the only procedure we'll ever need to use to do probabilistic inference-for the rest of this book and for the rest of our lives. To help keep the pieces organized, we'll arrange them in a table, which I'll refer to from now on as an inference table. The following are the steps for any problem, and the corresponding inference table is shown in table 1.1.

1. Enumerate all the possible hypotheses, $H_{1}, \ldots, H_{n}$ and consider their probabilities not including any observation, $P\left[H_{1}\right], \ldots, P\left[H_{n}\right]$. These are the prior probabilities, or priors for short.
2. For a given observation of data, $D$, compute the probability of that observation assuming each hypothesis is true, in turn. These are the sampling probabilities for the data given the hypotheses.
3. Compute the probability of arriving at the observation $D$ by means of any one of the hypotheses by multiplying the prior by the sampling probability: for example, $P\left[H_{1}\right] \cdot P\left[D \mid H_{1}\right]$ and so on. We'll call these the pathway probabilities. Summing them gives the total probability of the data:

$$
P[D]=P\left[H_{1}\right] \cdot P\left[D \mid H_{1}\right]+\ldots+P\left[H_{n}\right] \cdot P\left[D \mid H_{n}\right]
$$

TABLE 1.1 All-purpose inference table

| Hypothesis | Prior probability | Sampling probability | Pathway probability |
| :---: | :---: | :---: | :---: |
| $H_{1}$ | $P\left[H_{1}\right]$ | $P\left[D \mid H_{1}\right]$ | $P\left[H_{1}\right] \cdot P\left[D \mid H_{1}\right]$ |
| $H_{2}$ | $P\left[H_{2}\right]$ | $P\left[D \mid H_{2}\right]$ | $P\left[H_{2}\right] \cdot P\left[D \mid H_{2}\right]$ |
| $\ldots$ | $\ldots$ | $\cdots$ | $\cdots$ |
| $H_{n}$ | $P\left[H_{n}\right]$ | $P\left[D \mid H_{n}\right]$ | $P\left[H_{n}\right] \cdot P\left[D \mid H_{n}\right]$ |

4. Once this calculation is accomplished, the inferential probability for each hypothesis is easy to find, since it is just the relative proportion of that term in the preceding sum. These are the posterior probabilities, which, according to Bayes' theorem, are given by

$$
P\left[H_{i} \mid D\right]=P\left[H_{i}\right] \frac{P\left[D \mid H_{i}\right]}{P[D]}
$$

That is, the posterior probability for a hypothesis given data is the proportion of the total probability for the data represented by the pathway through that hypothesis. What this also means, practically, is that once we've computed the priors and the sampling probabilities, all the real work is done. The rest is just accounting.

With the aid of his theorem, Bayes was able to give a complete answer to the question he considered. A consequence of this inference was that future events could, under some assumptions, be logically predicted to have roughly the same chance of occurring as they had been seen to occur in the past. This showed, somewhat contrary to Hume's claims, that, through rational application of probabilities, one could arrive at knowledge from experience or at least something very close to knowledge—not absolute certainty as in a logical deduction, perhaps, but probable judgment in the sense of Cicero and the ancient Greeks. It wasn't a complete answer to the problem of induction, but it was close.

Whether Bayes himself believed he had disproved Hume we have no way of knowing. Some historians such as Stephen Stigler at the University of Chicago have suggested that since Bayes did not find the counterexample sufficiently convincing because it relied on some assumptions he could not justify, he delayed publishing his results. When presenting Bayes's results to the world, Price did not shy away from emphasizing their philosophical and religious significance. Contemporary reprints of the essay show Price intended the title to be "A Method of Calculating the Exact Probability of All Conclusions founded on Induction." ${ }^{17}$ In his publication, he added this preamble: "The purpose I mean is, to shew what reason we have for believing that there are in the constitution of things fixt laws according to which things happen, and that, therefore, the frame of the world must be the effect of the wisdom and power of an intelligent cause; and thus to confirm the argument taken from final causes for the existence of the Deity."18 That is, somewhere in the calculation of probabilities for Bayes's rule, Price thought he saw evidence for God.

Somewhat later, Pierre-Simon Laplace, apparently unaware of Bayes's solution, published his own version of the theorem and showed its application to
problems of inference. Laplace was, in our current sense, more Bayesian than Bayes himself had been, since Laplace was ready to divorce probabilities from frequencies or empirical fact altogether. The big question concerned the prior probabilities needed to do Bayesian inference: Where did these come from?

Bayes had confined himself to a problem where the prior probabilities are somewhat obviously uniform, like our target value probabilities in the earlier example. He had still broken new philosophical ground by showing probabilistic inference could go backward in time, but his treatment of probability suggested he considered these probabilities to exist independently of the person doing the analysis. Laplace allowed probabilities to depend on the observer's state of knowledge. He opened his treatise on the subject, Théorie analytique des probabilités (Analytical theory of probabilities), published in 1812, with this definition: "The probability for an event is the ratio of the number of cases favorable to it, to the number of all cases possible when nothing leads us to expect that any one of these cases should occur more than any other, which renders them, for us, equally possible."19 The "for us" made Laplace's probabilities subjective. This freed him up to compute inferential probabilities for all manner of propositions based on all manner of observations. As he described it, "Probability relates partly to our ignorance, partly to our knowledge."20

Laplace included, perhaps tongue-in-cheek, an example computing the probability the sun would rise tomorrow given it had risen every day in recorded history. With a general mathematical tool he called the rule of succession, he arrived at the probability $(d+1) /(d+2)$, where $d$ is the number of days of previous observation. Assuming, say, 5,000 years of recorded observations would give something like $d=1,825,500$, for a probability of 0.99999945205 .

The point was not so much the exact value as the fact it was less than 1 . Anything less than total certainty the sun would rise was seen as a ridiculous conclusion, and Laplace was roundly criticized for this, especially by frequentists like Venn. In The Logic of Chance, Venn wrote of this example, "It is hard to take such a rule as this seriously"21 because, among other reasons, the probability was manifestly wrong in the frequentist meaning, since it would not match the long-run frequency of occurrence.

However, his critics failed to properly understand that Laplace also rejected this conclusion as a misapplication of his rule! He had derived the rule of succession for inference problems about systems like Bernoulli's urn, where some unknown proportion of colored balls determines the single-event probability of a trial. Laplace included as an assumption that we begin from complete ignorance about the proportion, so we assign it a uniform probability of any value between 0 and 1 and assume that the resulting days, if given, are like
independent "draws" from the urn. However, in real life we know the sun is not such a system, and we have a great deal more understanding of the sun than just whether it has risen each day. In Laplace's own words: "But this number [the probability of the sun coming up tomorrow] is far greater for him who, seeing in the totality of phenomena the principle regulating the days and seasons, realizes that nothing at present moment can arrest the course of it."22 Laplace was not giving some objective probability the sun would rise but merely the subjective probability one would assign, consistent with Bayesian updating, starting from a position of total ignorance of what the sun even is.

Bayes loosened the lid on the idea of subjective probability, and Laplace removed it completely. Over the course of the next two centuries, many prominent philosophers and mathematicians took up the idea that probability meant the speaker's degree of belief in a given proposition. John Maynard Keynes took this position in his Treatise on Probability (1921), ${ }^{23}$ and Frank Ramsey defined probability in personalist terms in his essay "Truth and Probability" (1926). ${ }^{24}$ The British physicist Harold Jeffreys played perhaps the greatest role in preserving the Bayesian view of probability in science into the mid-20th century, applying Bayesian techniques with great success in the domain of geophysics and clarifying many of the practical considerations in his textbook Theory of Probability (1939). As Jeffreys wrote: "The essence of the present theory is that no probability, direct, prior, or posterior, is simply a frequency.".25

Philosophically speaking, there were a few major problems to overcome, though. One was that Laplace's definition of probability as a ratio of cases-and all the mathematics of probabilities that followed as a result-seemed unsupported. If we think of probabilities as ratios of equiprobable events, as in the classical definition, or as limiting frequencies, as in the frequentist definition, then these properties are self-evident. But if we are willing to scrap all of that and say probability is just a "degree of belief," measured on a scale from 0 percent to 100 percent, why should these axioms hold at all? If my degree of belief in the proposition "It will rain tomorrow" is 30 percent, why should that mean my degree of belief in "It will not rain tomorrow" is 70 percent? And if the basic property $P[A]=1-P[\operatorname{not} A]$ did not have to hold, what hope was there for Bayes' theorem or any other familiar mathematical result?

The Italian statistician and actuary Bruno de Finetti, working in the 1920s and '30s, attempted an answer by defining probability in terms of betting prices. Instead of a vague degree of confidence, he assumed the probability of an event could be made "operational" as the price the speaker would agree to pay for a bet of one unit on whether the event occurred. So a probability assignment of 30 percent for it raining tomorrow was equivalent to an agreed-upon price of
$\$ 0.30$ for a $\$ 1$ bet on whether it would rain, and so on. In a sense, this stayed faithful to the origins of probability in Pascal and Fermat's analysis of gambling games; Bayes, too, had phrased all his probabilities in terms of "expectations," meaning fair values of bets.

This concrete idea of probabilities then allowed de Finetti to impose additional structure that would constrain the probabilities a rational agent would give. The key idea was a Dutch book, a portfolio of bets that would earn a sure profit (in modern language, we would call this an arbitrage strategy). He showed that unless a person's probability assignments-that is, betting prices-followed the rules of probability, a Dutch book was always possible. For example, suppose my probability of it raining tomorrow were 30 percent, meaning I'd pay $\$ 0.30$ for a chance to win $\$ 1$ if it rained, but my probability of it not raining were 80 percent, so I'd pay $\$ 0.80$ to win $\$ 1$ if it didn't rain. Someone could make a Dutch book against me by selling me both bets for a total price of $\$ 1.10$ with the certain profit of $\$ 0.10$, since they would have to pay out only $\$ 1$ in either case.

Using similar assumptions about the coherence of bets placed over multiple times, de Finetti was even able to show Bayes' theorem for conditional probabilities had to hold. So the whole of mathematical probability was intact if probabilities were thought of as betting prices of a rationally coherent agent, meaning someone who was able to avoid price combinations that would make them certain losers.

However, another problem remained, which was that de Finetti's betting prices could still be totally arbitrary as long as they held together as a system of probabilities. That is, he could not tell anyone what price they should pay for a given bet. This obviously ran afoul of those instances of probability that seemingly could be verified empirically. Nothing would constrain a person, under the subjective definition, from believing they had a 1-in-30 chance of winning at roulette, instead of the conventional answer of 1-in-38, and proceeding to bet endlessly against unfavorable odds in a casino. Because they would probably lose but not certainly, de Finetti's assumptions didn't prevent this kind of thing from happening.

Similarly, a weather forecaster might predict a 99 percent chance of rain every day for a year and, after seeing only maybe 15 percent of those days turn out to be rainy, shrug off any criticism as a matter of different degrees of belief. Degrees of belief could be as personal as movie opinions and restaurant reviews. How could a subjective degree of belief ever be wrong?

Laplace had attempted to pin down probability assignments as the ratio of cases when there was no reason to prefer one case over another, which came
to be known as the principle of insufficient reason. Keynes rebranded it as the principle of indifference and emphasized that it applies only when we have no information suggesting unequal probabilities. But here, again, the objective versus subjective problem made itself known. Were the probabilities actually equal in fact, or do we just treat them as equal because we don't know any better? If the latter, then certainly there were examples where we'd compute the wrong answers through ignorance, contradicting empirical experience. Wasn't this a concern?

Also, an annoying technical problem came up when trying to apply the principle to continuous parameters (as even Bayes and Laplace had considered). The problem was that there seemed to be no consistent probability distribution for continuous values representing total ignorance. Suppose an unknown quantity had a continuous value-for example, the length of the side of a square sheet of paper known to be between 0 and 10 inches-but that's all the information we're given. We might say ignorance would force us to assume it is uniformly distributed, meaning it's just as likely to be in any range of a given size within the allowable limits. This would mean in particular that it had equal probabilities of being smaller or larger than 5 inches. But the same ignorance about the side length could equally well apply to the area of the square (or any other derived quantity), so total ignorance would imply the area, known to be between 0 and 100 square inches, should also have a 1/2 chance of being less than 50 square inches. However, since area and side length are related by the equation $A=S^{2}$, these two conclusions are inconsistent; the squares with side lengths less than 5 inches have areas less than 25 square inches, not 50. Clarification of how the principle of indifference would defend against these so-called Bertrand paradoxes-after the French mathematician Joseph Bertrand, who first introduced a similar problem in 1889 - would take a long time to develop (and in some cases is still ongoing). In the meantime, these problems caused logicians like Boole and Venn to reject the principle altogether in favor of objective frequencies.

## THE AXIOMATIC ANSWER

Advantages: Mathematically rigorous.

Disadvantages: Doesn't answer the question.

In 1900, the German mathematician David Hilbert gave an address to the International Congress of Mathematicians about what he considered to be the
most important outstanding problems at the time. Known ever since then as the Hilbert problems, the 23 challenges he issued (10 during the presentation and the rest in print) set the course of mathematics for the 20th century. They attracted the attention of the greatest mathematicians of the century, and those who contributed significantly to solving any of the problems reached an even higher echelon of greatness, becoming what mathematician Hermann Weyl called "the honors class."26

The second of these 23 problems was to prove that the axioms of arithmetic are consistent, and the sixth was to establish an axiomatic treatment of probability, as it was required for statistical physics. Both desires were in keeping with a great push in the mathematical community around that time to examine the foundations of mathematics and shore up parts of various disciplines long taken for granted. Most notably, Bertrand Russell and Alfred North Whitehead published their famous Principia Mathematica in three volumes over the period 1910-1913. Contained within was an attempt to formalize the rules of symbolic logic from which all mathematical truths could be derived.

It was against this backdrop that, in 1933, Russian mathematician Andreı Kolmogorov published his Foundations of the Theory of Probability, ${ }^{27}$ which was the first modern axiomatic treatment probability had received. His key idea was that probability could fit within the somewhat new mathematical domain called measure theory, developed over the late 19th and early 20th centuries by Émile Borel, Henri Lebesgue, and others. A measure in its most abstract form is a way of associating nonnegative numbers to subsets of a given master set in a way that satisfies certain constraints, such as the measure of the union of disjoint sets being the sum of the measures of each set. In Kolmogorov's translation, the master set, or sample space, would represent all the possible outcomes of some random situation or process, like the 216 possible outcomes of rolling three dice, and the subsets would be the possible events, like the dice summing to 9 or 10. The measure of a set would be the probability of that event occurring, standardized so that the measure of the whole space was 1.

Kolmogorov's axioms cleaned up a number of issues of theoretical probability, particularly questions having to do with infinite sets or infinite collections of sets. Using the powerful measure theory, Kolmogorov was able to prove several important theorems involving limits of sequences of random variables and other things that had vexed probability theorists for years, including a stronger version of Bernoulli's Law of Large Numbers.

However, the axiomatic system Kolmogorov developed, and all the rich, beautiful theory it entailed, did not answer the questions of where probabilities
came from in the first place or how to understand their meaning in the real world. Any example of a probability measure space would assume the basic probabilities had been given from the start. The axiomatic system could apply equally well to objective and subjective probabilities (at least granting something like de Finetti's ideas about coherent betting prices). It was clear from his writings that Kolmogorov thought of probabilities as frequencies, which made these axioms seem more natural, but there was nothing mathematically to disallow other interpretations.

## PROBABILITY AS LOGIC: THE SYNTHESIS

By the middle of the 20th century, philosophers, mathematicians, statisticians, and working scientists who used probability had rallied around Kolmogorov's axiomatization of the subject as a mathematical system, but there was still no general agreement on the interpretation of probability in any real problem. Instead, there seemed to be a patchwork of overlapping and somewhat related concepts, straddling the line between objective and subjective, between ontology (the study of things as they are) and epistemology (the study of our knowledge of things). Sometimes probability meant empirical frequency, as most statistical practice would have it (more on this later), and sometimes it meant subjective degree of belief, as Laplace and his Bayesian descendants would use it in problems of inference. Frequency interpretations seemed to be more suitable for games of chance or repeated randomized experiments such as sampling randomly from a population. Degrees of belief seemed more applicable to forecasting one-time events, testing hypotheses, and making inferences about the past. Most probability textbooks tried to remain as neutral as possible on the subject and move swiftly to proving results about probability measure spaces and random variables. No single definition of probability seemed adequate to cover all these cases.

Indeed, for many people this is how the story ends, with probability simply meaning different things at different times or in different applications. Any way of assigning numbers to subsets of some sample space in a way that satisfied Kolmogorov's axioms could be called a probability, and all the mathematical properties one could want (and then some) would come for free. So what harm is there in sometimes applying the idea to proportions of a set of equiprobable outcomes and sometimes applying it to betting prices assuming coherence and sometimes applying it to limiting frequencies of a series of experiments?

Well, one major way this causes harm, as we'll see abundantly, is through the confusion it causes when the concepts are mixed together, particularly for scientific inference. Our assessment of the probable truth of a hypothesis is clearly subjective, but it's constructed using sampling frequencies for the data, which are objective. When subjective combines with objective, which one trumps the other?

However, there were some in the late 20th century who continued to seek a synthesis, a way of interpreting frequency-based probability and belief-based probability as different instances of the same underlying phenomenon. The closest anyone had come thus far had been in 1921, when Keynes published his logical theory of probability, including the principle of indifference. So logic was where these new authors began. But a new form of logic was clearly needed because classical logic dealt only with certain deductions, not probabilities. As the physicist James Clerk Maxwell had described in 1850, probabilistic thinking was more natural in some ways than classical logic anyway because no proposition in the real world is ever truly certain: "The actual science of logic is conversant at present only with things either certain, impossible, or entirely doubtful, none of which (fortunately) we have to reason on. Therefore the true logic for this world is the calculus of Probabilities, which takes account of the magnitude of the probability which is, or ought to be, in a reasonable man's mind.".28

Keynes had attempted to define probability as a "degree of rational belief," 29 and some practitioners continued to argue for this definition and to make more precise the source of that rational belief. For example, Harold Jeffreys defined probability as the support one proposition gives to the truth of another: "We introduce the idea of a relation between one proposition $p$ and another proposition $q$, expressing the degree of knowledge concerning $p$ provided by $q .{ }^{\prime 30}$ But still there was the question of why the mathematical laws of probability should hold. As Ronald Fisher wrote in a 1934 article, part of a series of back-and-forth arguments with Jeffreys:

Keynes establishes the laws of addition and multiplication of probabilities, by stating these laws in the form of definitions of the processes of addition and multiplication. The important step of showing that, when these probabilities have numerical values, "addition" and "multiplication," as so defined, are equivalent to the arithmetical processes ordinarily known by these names, is omitted. The omission is an interesting one, since it shows the difficulty of establishing the laws of mathematical probability, without basing the notion of probability on the concept of frequency, for which these laws are really true, and from which they were originally derived. ${ }^{31}$

For example, the only reason the probabilities of the event $A$ and the event (not $A$ ) add up to 100 percent is that proportions behave that way.

This was the real problem at the heart of the feud between the different interpretations of probability: there was a strong case to be made that a frequency and proportion understanding of probability was inadequate for all situations, but the agreed-upon axiomatic system was based on these elementary frequency and proportion concepts. If probability was not somehow defined in reference to proportions, why should the rigid axioms of Kolmogorov's mathematical probability, and all the theory that depended on them, be expected to hold true? What would stop us from assigning whatever degree of belief we wanted to any proposition?

De Finetti's Dutch book argument had shown that the rational prices we would agree to pay to bet on propositions would need to obey the rules of probability, but that interpretation left two major holes. For one thing, it couldn't say if a probability was right, and without resorting to long-run frequencies, we have no other basis for coming up with these numbers. Second, and somewhat relatedly, the probability we associate to an event might not match the price we'd pay to bet on it. People are willing to play gambling games at prices significantly higher than their pure expected value based on the probability of winning; this is what keeps casinos and state lotteries in business. That doesn't mean we should change our probability assignment, just that it must come from somewhere else.

The biggest breakthrough toward uniting the two interpretations came in 1979, when the American physicist Richard Cox proved the mathematical result now called Cox's theorem. The main idea was this: start over from scratch, and think of probabilities not as relative measures of some subsets of a sample space, as Kolmogorov had done, but rather as degrees of plausibility given to propositions, more in line with the subjective interpretation. However, to keep these numbers internally consistent, Cox added the requirement that they respect the propositional calculus of ordinary logic and obey other principles in agreement with common sense.

Cox loosened the rigid requirement that the probability of proposition $A$ and the probability of proposition (not $A$ ) sum to 1 , saying only that if the plausibility of $A$ was given, the plausibility of (not $A$ ) should be determined. So the plausibility of $A$ could be 40 percent, say, while the plausibility of (not $A$ ) could be 80 percent-but only if anytime another proposition $B$ had a plausibility 40 percent, we'd also have a plausibility of (not $B$ ) equal to 80 percent. There was just some fixed rule that would get you from the 40 percent to the 80 percent.

Furthermore, Cox required these plausibilities to behave in such a way that if $A$ became more plausible, (not $A$ ) would become less so. This seemed like commonsense behavior for the plausibility of propositions and their negationshaving greater confidence in $A$ is the same as having less confidence in (not $A)$-and importantly this was not based on any idea of probabilities as proportions. Similarly he assumed that if the plausibility of $A$ and the plausibility of $B$ given $A$ was known, then the plausibility of $(A$ and $B$ ) would be determined, and if either ingredient became more plausible, the combination would likewise become more plausible.

From these and other similar assumptions about how plausibilities of propositions should behave (plus other technical conditions on the mathematical functions involved), Cox was able to show there always exists a way of rescaling his plausibilities such that the rescaled values satisfy the familiar axioms of probability. In other words, probability became a convenient system of units to describe plausibilities with nice mathematical properties, like using degrees Kelvin to describe temperature instead of degrees Fahrenheit. This gave an entirely new justification for Kolmogorov's axioms that had nothing whatsoever to do with frequencies or relative proportions and that was also free of the artificiality of de Finetti's coherent betting prices.

The most complete synthesis was achieved by Edwin Jaynes, another American physicist, beginning with a series of papers in the 1980s and culminating in his survey Probability Theory: The Logic of Science, ${ }^{32}$ published posthumously in 2003. He was for many years a professor of physics at Washington University in St. Louis and had already made a career studying statistical mechanics and particle physics separately from his interest in theoretical probability. But his practical experience as a scientist-particularly in these domains, where probability had made great inroads - led him to believe there was something missing in the way most practitioners thought about probability.

In Jaynes's view, probability was entirely about information-specifically, the degree of certainty a rational person should have given incomplete information about an event or process. Anyone who attempted to make it "objective" by defining probability in terms of empirical frequencies was committing what he called the "mind projection fallacy"33 - that is, confusing the speaker's mental state with the objective facts of the outside world. He rejected entirely the idea of verifying probabilities empirically; he said this would be "like trying to verify a boy's love for his dog by performing experiments on the dog."34

Instead, having been motivated by Cox's result and drawing further inspiration from George Pólya's writings about the way mathematicians reason in
practice, Jaynes defined probabilities as plausibilities satisfying certain commonsense properties similar to Cox's, rescaled (per Cox's theorem) so that the familiar equations of probability would hold true. Jaynes emphasized the role of the background information these probabilities depended on by always including a "conditional on $X$ " in the notation, where $X$ captured the assumptions of that problem. So, for example, Jaynes's version of the rules of probability included two main calculation rules, the sum rule:

$$
P[A \mid X]+P[\operatorname{not} A \mid X]=1
$$

and the product rule:

$$
P[A \text { and } B \mid X]=P[A \mid X] \cdot P[B \mid A \text { and } X]
$$

Depending on your background, these equations may be anywhere from trivial to mystifying, but really the ideas are simple and familiar. The first rule expresses the basic fact that the probability of a proposition and its negation must sum to 1 . That concept is obvious for proportional measures of probability, but here it is the result of rescaling plausibilities so that these equations hold true. Once you have "unlearned" the idea that probability means proportion, it takes a substantial amount of work to get back to this "obvious" equation.

We already encountered the second equation, without the "conditional on $X$ " decoration, when we discussed Bayes' theorem. The proposition ( $A$ and $B$ ) could refer, say, to a particular person having two characteristics simultaneously; the ingredients on the right-hand side are then the probability of having one characteristic and the conditional probability of having the second one assuming the first one. The notation expressing all these statements as "conditional on $X^{\text {" }}$ is Jaynes's innovation, but it captures a simple yet powerful idea: that all three probabilities are dependent on some underlying state of knowledge making us uncertain about this particular person in some way.

But Jaynes did not just allow for arbitrary assignments of probabilities, in the loosest subjectivist sense. Instead, he required probabilities to satisfy constraints that depended on the information assumed in any given problem. He did this by considering the possible transformations of the background information and the implications these might have for probability assignments. If, for instance, a problem could be transformed into another problem in such a way that the person doing the probability assignment was in the same state of knowledge, the probabilities they assigned must be the same.

A simple example would be drawing a ball from an urn containing two balls-say one black and one white. Letting $A$ be the proposition "We draw the black ball" and $B$ be the proposition "We draw the white ball," we might imagine a state of information that consists only of proposition $X$ : "Exactly one of $A$ or $B$ is true." However, if we interchange the labels $A$ and $B$, proposition $X$ would be transformed into $X^{\prime}=$ "Exactly one of $B$ or $A$ is true." Since this is logically an equivalent statement to our original $X$, we are in the same state of information. In summary, switching the proposition we called $A$ with the one we called $B$ had no effect on our state of knowledge. According to Jaynes, this means that, conditionally only on $X$, propositions $A$ and $B$ must have the same probability. And since they're mutually exclusive and exhaust all the possibilities in this problem, their probabilities must also sum to 1, meaning both $A$ and $B$ have probability $1 / 2$ given $X$. That is, in Jaynes's notation, $P[A \mid X]=P[B \mid X]$ $=1 / 2$. Different states of information might give rise to different probabilities. For example, we could have had background knowledge that the black ball was on top and we would draw from the top; this would result in $A$ being certain, while $B$ is impossible.

Jaynes even imagined this kind of reasoning being programmed into a robot, so probabilities would become nothing more than a dispassionate numerical processing of the available information loaded up as assumptions of a given problem. This mirrored similar initiatives in the world of computer science to represent logical reasoning, meaning deductive proof, as Boolean algebra, the arithmetic of ones and zeros native to digital computers.

In fact, Jaynes's version of probability as logic showed that probability calculations are simply extensions of logical deduction from true-or-false arithmetic to computation with other numbers. For example, a basic step of deductive logic called the rule of contraposition is that the implication " $A$ implies $B$ " is logically equivalent to the implication "(not $B$ ) implies (not $A$ )." If we know that whenever it rains $(A)$, Mr. Smith always takes the bus to work $(B)$ and we see one day that he did not take the bus (not $B$ ), then we are logically justified in concluding it must not be raining ( $\operatorname{not} A$ ).

We can describe this deduction as a special case of Bayes' theorem. Thinking of the proposition (not $A$ ) as our hypothesis and the proposition (not $B$ ) as our data, according to the usual procedure, to see what consequence the data has for our hypothesis, we need to consider all the pathways to the data to calculate the posterior probability for the hypothesis given the data. But the only pathway other than the one through (not $A$ ) goes through the proposition $A$, which we know gives a sampling probability for (not $B$ ) equal to 0 ,
since $P[B \mid A]$ is 1 . Therefore, when we express the pathways as relative proportions, the probability of $(\operatorname{not} A)$ given $(\operatorname{not} B)$ is 1 . In other words, given $(\operatorname{not} B)$, ( not $A$ ) is certain, the rule of contraposition.

Other basic deductive rules like the rule of modus ponens-if we are given the premise " $P$ implies $Q$ " and that $P$ is true, we conclude $Q$ is true-follow by similar reasoning. In this way, logical deduction is just a special case of reasoning with probabilities, in which all the probability values are zeros or ones.

## THE DIFFERENCE BETWEEN VALIDITY AND TRUTH

Jaynes's criticism of the frequentists was extremely harsh. First, he not so politely asked them to stop using the word probability if they were just going to mean frequency anyway because this was nowhere near faithful to all the ways probability had been used in making judgments (as in Cicero's "guide to a wise person's life") since before mathematical probability even existed. He suggested their misuse was only confusing everyone:

It seems to us that, if $\mathrm{Mr} \mathrm{A}$ wishes to study properties of frequencies in random experiments and publish the results for all to see and teach them to the next generation, he has every right to do so, and we wish him every success. But in turn Mr B has an equal right to study problems of logical inference that have no necessary connection with frequencies or random experiments, and to publish his conclusions and teach them. The world has ample room for both. Then why should there be such unending conflict, unresolved after over a century of bitter debate? Why cannot both coexist in peace? What we have never been able to comprehend is this: If Mr A wants to talk about frequencies, then why can't he just use the word "frequency"? Why does he insist on appropriating the word "probability" and using it in a sense that flies in the face of both historical precedent and the common colloquial meaning of that word? By this practice he guarantees that his meaning will be misunderstood by almost every reader who does not belong to his inner circle clique. ${ }^{35}$

But Jaynes would certainly admit some repeated experiments like flipping coins or rolling dice did result in stable frequencies. His point was that these frequencies actually are properties of those physical systems (including, most importantly, the variability in the initial conditions-the position, velocity, angular momentum, etc. of all the objects in play) that exist independently
of the person doing the probability calculation. The probability could not be measured, but the frequency could be.

Why should probability and frequency ever give the same number? Because, Jaynes argued, we assign probabilities for these physical systems based on a lot of detailed knowledge of them, including their previously observed frequencies! That is, for an example such as flipping a coin, we know a lot about coins, including that they are (roughly) physically symmetric, and we know a lot about what it means to flip them, including that the initial conditions when thumb is applied to coin are somewhat uncontrollable and that the outcome depends very sensitively on what happens in that instant. Therefore, we correctly process our ignorance of the initial conditions of a particular coin flip, along with our other knowledge of the symmetry of the coin, into a 50/50 probability for that flip coming up heads.

This also gave Jaynes a way to address examples of extremely rare events, like our all-spades bridge hand. We know, from practical experience handling cards, that they are roughly identical apart from the number and suit printed on each one, and we know that those differences don't affect how any particular card moves around when shuffled in a deck. Furthermore, we know that tiny differences in the exact mechanical details of each individual shuffle accumulate to large differences in the final order of cards.

So our knowledge of those physical aspects of the cards, combined with our understanding of the chaotic nature of the shuffling process and our ignorance of all the fine details of a particular shuffle, leads us to assign the probability $13 / 52$ to the first card dealt being a spade, the conditional probability 12/51 to the next, and so on until we arrive at the astronomically low chance of being dealt all 13 spades we computed previously. That realm of "symmetric ignorance" is the place these calculations originate from, and our agreement on the nature of that ignorance is what makes us so confident in them that even a billion years of observed card dealing could never persuade us otherwise.

In particular, the number we came up with for the probability would be our answer whether we understood that the process was going to be repeated or whether we expected that it would happen only one time, after which the deck would be thrown into the fireplace and destroyed. In this way of thinking, we don't have to imagine an impossible series of card shuffles to confirm for ourselves that our probability calculation is correct.

However, we might, for various reasons, be led to ask what we expect the long-run frequency of this bridge hand to be if, hypothetically, a long series of similar shuffles were possible. The same argument we used to deduce the
one-time probability could be extended with the extra observation that we don't have any information to connect the results of one shuffle of the deck with the results of any other. That is, in our understanding of cards and how they work, we would assign successive shuffles probabilities as though they are independent. Putting this together with our previous answer and a Bernoulli-esque Law of Large Numbers argument, we would expect within some small margin (and with high but not perfect confidence) that, for a very long series of trials, the frequency we'd observe would match our probability answer for the bridge hand.

It might seem that we've just argued in a circle. We can't simply say the probability of getting an all-spades hand is equal to the long-run frequency (as the frequentist interpretation would suggest we must) because it's impossible to actually do such an experiment and as a result we don't know the frequency. But we do know certain things about the physical properties of cards that allow us to give a probability answer anyway, which, as it turns out, is equal to what we think the frequency probably is. So we do sort of know the frequency.

But here's the difference: we based our probability answer not on an assertion that it's the frequency we would obtain but rather on the tangible facts about cards that we know are true from actual experience. The logical dependency goes like this:

Known facts about cards $\Rightarrow$ One-time probability of a perfect bridge hand $\Rightarrow$

Predicted frequency of this hand occurring over the theoretical long run

whereas the frequentist answer is something more like this:

“Known" frequency of this hand occurring over the theoretical long run (?) $\Rightarrow$ One-time probability answer (by definition)

Furthermore, and most importantly, we could hold those assumptions of symmetry provisionally as a hypothesis and allow practical experience to change our minds as evidence accumulates. So we might say, for example, that we're pretty sure the results of a shuffle don't influence the results of the next one, but if we checked our theoretical predictions against observation, we might become less sure. The frequentist interpretation has no such wiggle room.

According to Jaynes, probabilities are a consequence of the assumptions present in the background. And the assumptions we make might be incorrect. For example, say a person with no knowledge of magicians or sleight of hand were asked for the probability that someone could blindly draw a particular
card from an apparently well-shuffled deck. They would be perfectly justified in giving the answer $1 / 52$, consistent with their background knowledge. If a magician then exhibited this ability over and over, it wouldn't make the person's probability calculations wrong, just founded on ignorance. Similarly, for any of our urn-drawing examples, we might reach in and find the urn is empty! This doesn't mean our calculation was incorrect. Our probability robot processed the inputs given to it in the correct way; it's just that we may have given it garbage and should expect garbage in return, as is the case with every algorithm.

Exactly the same phenomenon occurs in ordinary logic: a deduction may be valid, meaning it appropriately follows the rules of deduction, yet lead to a false conclusion because one or more of the premises are false. For example,

If it's Wednesday, there was once life on Mars.

It's Wednesday.

$\therefore$ There was once life on Mars.

is a valid deduction even though the premise is faulty and it may not even be Wednesday.

In the probability-as-logic interpretation, our probability assignments do not need to be right, in the sense of being verifiable externally by some experiment; they need only to be a valid expression of the information we are given and the assumptions we hold to be true.

Trying to force probability answers to be right or wrong by claiming probabilities were the frequencies one "would" obtain as the limit in an infinite number of trials especially annoyed Jaynes, who had years of practical experience as an experimental physicist. He chastised mathematicians sharply for fabricating these claims out of pure thought-imagining all experiments as drawing from some "infinitely large urn" if need be-and then trying to claim they had done so objectively:

In other cases, such as flipping a coin, making repeated measurements of the temperature and wind velocity, the position of a planet, the weight of a baby, or the price of a commodity, the urn analogy seems so farfetched as to be dangerously misleading. Yet in much of the literature one still uses urn distributions to represent the data probabilities, and tries to justify that choice by visualizing the experiment as drawing from some "hypothetical infinite population" which is entirely a figment of our imagination. Functionally, the main consequence of
this is strict independence of successive draws, regardless of all other circumstances. Obviously, this is not sound reasoning, and a price must be paid eventually in erroneous conclusions. This kind of conceptualizing often leads one to suppose that these distributions represent not just our prior state of knowledge about the data, but the actual long-run variability of the data in such experiments. Clearly, such a belief cannot be justified; anyone who claims to know in advance the long-run results in an experiment that has not been performed is drawing on a vivid imagination, not on any fund of actual knowledge of the phenomenon. Indeed, if that infinite population is only imagined, then it seems that we are free to imagine any population we please. ${ }^{36}$

As Jaynes suggested, no probabilist would ever hold themselves to such a standard anyway because no limiting frequencies had ever really been observed or ever would be:

Unfortunately, to maintain [the frequentist] view strictly and consistently would reduce the legitimate applications of probability theory almost to zero; for one can (and most of us do) work in this field for a lifetime without ever encountering a real problem in which one actually has knowledge of the "true" limiting frequencies for an infinite number of trials; how could one ever acquire such knowledge? Indeed, quite apart from probability theory, no scientist ever has sure knowledge of what is "really true"; the only thing we can ever know with certainty is: what is our state of knowledge? ${ }^{37}$

So frequentist probability was, in Jaynes's view, complete nonsense. It existed primarily as a way for scientists to maintain a self-satisfied notion of objectivity and sidestep the question of what background knowledge and preconceptions they were bringing to any given problem.

Jaynes's notion of probability as logic made the importance of these assumptions explicit while simultaneously showing his theory could reproduce all the frequentist results if loaded up with background assumptions consistent with the real physical behavior of the apparatus of the random experiment. In this way, he achieved a synthesis of subjective and objective probability.

The point was that if our background assumptions had a kind of symmetry, our probabilities would also have to have this symmetry and thus be forced to have particular numerical values. Jaynes formalized the principle of indifference Keynes had postulated (for Jaynes, it was a theorem), and in doing so, he split the difference between the subjective and the objective. Jaynes's
probabilities were subjective in the sense of being dependent on the assumptions brought to a problem by a particular person, but they were objective in the sense that any two people reasoning rationally (following Cox's rules for plausible reasoning) from the same starting assumptions would necessarily arrive at the same answer.

The real power of this interpretation of probability first starts to become apparent when we apply it to problems of inference, as in the problems that motivated Bayes and Laplace. Remember, one of the questions gestured at but left unanswered in those problems was where the prior probabilities came from. Bayes had constructed his example so the priors were manifestly uniform, and Laplace had assumed them mostly as a mathematical convenience.

In the Jaynesian view, there is no difference between prior probabilities and any other kind of probability. We are justified in assigning uniform probabilities any time our background knowledge makes us indifferent between the various propositions-that is, if we have no information to lead us to prefer one or the other. This is exactly the same justification that leads us to assign sampling probabilities, like saying our chance of rolling a 6 with a fair die is 1/6. As Jaynes pointed out, the latter is usually easier to do only because the information about the sampling process has been specified more clearly than the background assumptions have:

From the start it has seemed clear how one determines numerical values of sampling probabilities, but not what determines the prior probabilities. In the present work we shall see that this was only an artifact of an unsymmetrical way of formulating problems, which left them ill-posed. One could see clearly how to assign sampling probabilities because the hypothesis $H$ was stated very specifically; had the prior information $X$ been specified equally well, it would have been equally clear how to assign prior probabilities. ${ }^{38}$

But according to Jaynes, specifying the information that determined these prior probabilities was crucial to any problem of inference. We could no more hope to make an inference without priors than we could hope to make an inference without data.

As an exercise in this way of thinking, and for a bit of fun, let's see how probability as logic handles a couple of the most famous paradoxes of probability that usually give headaches to students (and teachers!) in traditional probability courses. In each example, we'll see that the hard work we need to do to clarify and make explicit the background information we have when making
the probability assignments is all front-loaded. The actual conclusions will follow almost immediately.

## THE BOY OR GIRL PARADOX

This problem has been part of the lore of probability theory since at least 1959, when Martin Gardner published it in Scientific American: ${ }^{39}$

Mr. Smith says, "I have two children and at least one of them is a boy." What is the probability that the other child is a boy?

Although it may not appear so at first, this has the structure of a hypothesis test. We are interested in the hypothesis "Both children are boys," and we have some observed data: at least one of the two children is a boy. So we can apply Bayes' theorem (with Jaynes's notation) as with any hypothesis and data propositions:

$$
P[H \mid D \text { and } X]=P[H \mid X] \frac{P[D \mid H \text { and } X]}{P[D \mid X]}
$$

As Jaynes instructs us, we therefore must first consider our prior probability assignments. Knowing nothing other than the fact that someone has two children, what probability do we assign to our hypothesis? It is almost certainly the intent of the problem that we take this probability to be $1 / 4$. However, it may be worth inspecting that assumption a bit. There are four possible cases we can imagine, ${ }^{40}$ but do we necessarily consider them equally likely? For ease of reference, imagine we think of the older of the two as child 1 and the younger as child 2; we can then label the propositions as follows:

$B_{1}=$ "The older child is a boy"; $G_{1}=$ "The older child is a girl"

$B_{2}=$ "The younger child is a boy"; $G_{2}=$ "The younger child is a girl"

And we have the four cases:

$B_{1}$ and $B_{2}$

$B_{1}$ and $G_{2}$

$G_{1}$ and $B_{2}$

$G_{1}$ and $G_{2}$

If we know only that exactly one of these four cases holds true, then a Jaynesian transformation argument (say switching the labels $B_{1}$ and $G_{1}$ or $B_{1}$ and $B_{2}$ ) tells us our state of knowledge makes us indifferent to the four. Therefore, we must assign them each probability $1 / 4$.

However, in reality we probably know much more than that! We could, if we were so inclined, find actual rates of occurrence of (boy, boy) sibling pairs and so on, and we may find not all four combinations appear equally often. They would, at minimum, be somewhat confounded by the incidence of identical twins sharing a gender. At any rate, since it's not supposed to be the point of the problem, let's just assume that whatever state of information we have initially can at least be well approximated by one in which we assign each case probability $1 / 4$. These are our prior probabilities for these various propositions.

In true Jaynesian fashion, though, once we have done this work of assigning prior probabilities, the rest of the problem is pretty trivial. Suppose we represent the data proposition as:

$$
D=\text { "At least one child is a boy" }
$$

Our hypothesis, "Both children are boys," is just the case $\left(B_{1}\right.$ and $\left.B_{2}\right)$. Using our general template of Bayesian inference, we can build table 1.2. Here, all the sampling probabilities are 1 or 0 , since whether at least one of the children is a boy is determined deductively in each case. As a relative proportion, the pathway we care about, corresponding to the hypothesis $\left(B_{1}\right.$ and $\left.B_{2}\right)$, represents $(1 / 4) /(3 / 4)=1 / 3$ of the sum. So, as before, our posterior inferential probability for the hypothesis $\left(B_{1}\right.$ and $\left.B_{2}\right)$ given the data is $1 / 3$.

TABLE 1.2 Boy or girl paradox: at least one child is a boy

| Hypothesis <br> $H$ | Prior <br> probability <br> $P[H \mid X]$ | Sampling <br> probability <br> $P[D \mid H$ and $X]$ | Pathway <br> probability <br> $P[H \mid X] P[D \mid H$ and $X]$ | Relative <br> proportion <br> $P[H \mid D$ and $X]$ |
| :---: | :---: | :---: | :---: | :---: |
| $B_{1}$ and $B_{2}$ | $1 / 4$ | 1 | $1 / 4$ | $1 / 3$ |
| $B_{1}$ and $G_{2}$ | $1 / 4$ | 1 | $1 / 4$ | $1 / 3$ |
| $G_{1}$ and $B_{2}$ | $1 / 4$ | 1 | $1 / 4$ | $1 / 3$ |
| $G_{1}$ and $G_{2}$ | $1 / 4$ | 0 | 0 | 0 |

Most people are surprised at this result at first because we are so thoroughly conditioned to think the gender of someone unknown to us-in this case, the "missing" child-should be a 50/50 proposition. But the point here is the information "at least one child is a boy" is a weird kind of observation to have, and it puts us in a funny position where we can rule out only one of four possible cases, leaving the other three equally likely. If it had been phrased as "It is not the case that both children are girls," the inference would be more clear. ${ }^{41}$

To see a more "normal" situation, imagine we are given instead that Mr. Smith's older child is a boy-that is, $D=B_{1}$.

Then our inference table would look like table 1.3. And our posterior probability for $\left(B_{1}\right.$ and $\left.B_{2}\right)$ would be $(1 / 4) /(1 / 2)=1 / 2$. That is, given the gender of a particular child, we assign equal probabilities for the gender of the other child, in keeping with ordinary common sense.

We can even imagine different states of background knowledge or different kinds of information that could shift the probabilities around. For example, maybe instead of knowing directly that Mr. Smith has at least one boy, we could have the data proposition $D=$ "Mr. Smith tells us he has at least one boy." Now the problem becomes much more complex because our given observation involves the actions of a person, so we need to consider what we know about this person and his behavior. Our background assumptions could incorporate knowledge about Mr. Smith, such as an assumption that he had always wanted a daughter and would surely tell us at every opportunity if he had a girl. Under those assumptions, we have sampling probabilities for hypothesis ( $B_{1}$ and $G_{2}$ ) and hypothesis $\left(G_{1}\right.$ and $B_{2}$ ) equal to 0 . And our inferential probability for $\left(B_{1}\right.$ and $B_{2}$ ) equals 1! That is, deductively, we could reason that Mr. Smith passed

TABLE 1.3 Boy or girl paradox: the older child is a boy

| Hypothesis <br> $H$ | Prior <br> probability <br> $P[H \mid X]$ | Sampling <br> probability <br> $P[D \mid H$ and $X]$ | Pathway <br> probability <br> $P[H \mid X] P[D \mid H$ and $X]$ | Relative <br> proportion <br> $P[H \mid D$ and $X]$ |
| :---: | :---: | :---: | :---: | :---: |
| $B_{1}$ and $B_{2}$ | $1 / 4$ | 1 | $1 / 4$ | $1 / 2$ |
| $B_{1}$ and $G_{2}$ | $1 / 4$ | 1 | $1 / 4$ | $1 / 2$ |
| $G_{1}$ and $B_{2}$ | $1 / 4$ | 0 | 0 | 0 |
| $G_{1}$ and $G_{2}$ | $1 / 4$ | 0 | 0 | 0 |

up an opportunity to mention a daughter, so he must not have one, per our assumptions about him.

Likewise, we could imagine all kinds of fanciful scenarios about how we got this information, such as $D=$ "We rang the doorbell of Mr. Smith's house and a boy answered the door." Then we need to consider the impact of different assumptions about Mr. Smith's household door-answering policies, such as "If Mr. Smith had a son, his son would always answer the door" [posterior probability for $\left(B_{1}\right.$ and $\left.B_{2}\right)=1 / 3$ ] versus "Mr. Smith's children would answer the door equally often" [posterior probability for $\left(B_{1}\right.$ and $\left.B_{2}\right)=1 / 2$ ].

Another variant comes about if we assume something particular about the boy in question, such as $D=$ "At least one child is a boy born on a Tuesday." Following similar reasoning as previously (and with the same caveats), we could argue our way into probability $1 / 7$ under either "one boy" hypothesis and into something like probability $1-(6 / 7)^{2}$ assuming two boys, since the chance in a two-boy family of having at least one born on a Tuesday is the chance they're not both born on some other day. Our posterior probability for $\left(B_{1}\right.$ and $\left.B_{2}\right)$ then turns out to be the very surprising number $13 / 27$, or about 48 percent. This suggests the general pattern that the more specific information we know about this mystery "at least one" boy, the closer we are to pinning him down to being a particular one of the children, leaving us in the familiar situation of knowing one child's gender and assigning a 50/50 chance for the other's.

## THE MONTY HALL PROBLEM

This problem is likewise now legendary in probability circles. First posed in a letter to American Statistician in 1975 and made famous by Marilyn vos Savant in her "Ask Marilyn" column in Parade magazine in 1990, it's a slightly abstracted version of a situation faced by contestants on the game show Let's Make a Deal, hosted by Monty Hall from 1963 to 1976 (and occasionally in various revivals thereafter):

Suppose you're on a game show, and you're given the choice of three doors: Behind one door is a car; behind the others, goats. You pick a door, say door 1 , and the host, who knows what's behind the doors, opens another door-say door 3, which has a goat. He then says to you, "Do you want to pick door 2?" Is it to your advantage to switch your choice? $?^{42}$

In her column, vos Savant said you should switch, and by doing so, you would increase your chance of winning from $1 / 3$ to $2 / 3$.

Intuition may suggest it doesn't matter whether you switch because there are two remaining doors that can be hiding the car and it seems you have no reason to prefer one or the other. Many, many people saw it that way at the time, and they expressed no small amount of contempt toward vos Savant for claiming otherwise. She received over 10,000 letters about the problem and devoted three subsequent columns to defending her answer. Among those attacking here were numerous people with advanced degrees in math and statistics. For example, one math professor wrote, "As a professional mathematician, I'm very concerned with the general public's lack of mathematical skills. Please help by confessing your error and, in the future, being more careful." ${ }^{33}$ Someone with a $\mathrm{PhD}$ wrote, "You blew it, and you blew it big! Since you seem to have difficulty grasping the basic principle at work here, I'll explain. After the host reveals a goat, you now have a one-in-two chance of being correct. Whether you change your selection or not, the odds are the same. There is enough mathematical illiteracy in this country, and we don't need the world's highest IQ propagating more. Shame!"44 Another professor wrote, "Our math department had a good, self-righteous laugh at your expense." 45 Another PhD wrote, "May I suggest that you obtain and refer to a standard textbook on probability before you try to answer a question of this type again?"46 And yet another wrote, "You made a mistake, but look at the positive side. If all those Ph.D.'s were wrong, the country would be in some very serious trouble. ${ }^{147}$ Even the great mathematician Paul Erdős was thoroughly convinced switching didn't matter. However, all the PhD's were wrong, and vos Savant was right. Switching doors does improve your chance of winning from $1 / 3$ to $2 / 3$, as we can now show using Bayes' theorem.

As in the Boy or Girl Paradox, though, before computing any probabilities, we must faithfully account for our assumptions about what we have just seen and the circumstances in which we imagine ourselves. We can structure our analysis, again, as an inference about a hypothesis: in this case, the hypothesis that our chosen door was correct, conditional on some observations-namely, everything else given in the problem. However, since the content of our observations is more complex than in the last problem, some subtle considerations emerge when we start trying to write things out.

Let $H_{1}$ be the hypothesis that the car is behind door 1, with $H_{2}$ and $H_{3}$ similar. For starters, we'd like to say our prior probability assignment for $H_{1}$ is $1 / 3$. Why is this? One argument might be indifference; we were given only that the car was behind one of the three doors, so it feels like our ignorance is symmetric.

However, in a real-life situation we could also have come to this probability through repeated observation of the show. Maybe we know the car is more often behind door 1 because the producers prefer it that way. Or maybe we know the producers do a poor job of randomizing the car's location and never repeat the same door from week to week; this might lead us to higher levels of confidence in the car's location. Since none of this was specified in the problem, though, we'll assume indifference and assign the probability $1 / 3$.

Similarly, we need to think a little carefully about what it is we have actually observed. A faithful record of all of the observations given in the problem would be something like this:

## $D=$ "The host opened door 3" and "Door 3 revealed a goat" and "The host offered a switch to door 2"

We can eliminate $\mathrm{H}_{3}$ immediately, since that would be inconsistent with our observation -that is, the probability of this observation conditional on the car being behind door 3 is 0 . The subtlety emerges in assigning the sampling probabilities for $D$ given $H_{1}$ and $H_{2}$, and this is where the usual statement of the problem and the usual solutions tend to leave out some important details.

Under assumption $H_{1}$, the car is behind our chosen door 1, so we know the host has a choice of which other door to open, door 2 or door 3 . Do we have any reason to suspect he prefers one or the other? Nothing is stated in the problem, so we'll go ahead and assume indifference here as well, but, again, we could imagine having information that might guide us. Similarly, and more problematically, we will assume the host will surely offer the switch no matter what-maybe we know this to be a rule of the show. But nothing in the problem as stated explicitly gives us this information. We'll return to this assumption in a moment.

For now, though, we will make these assumptions, which are the standard ones given in most solutions. With these in place, we have all the necessary ingredients for our inference, since we can say our state of knowledge $X$ is such that

$$
P\left[H_{1} \mid X\right]=P\left[H_{2} \mid X\right]=P\left[H_{3} \mid X\right]=1 / 3
$$

and

$$
P\left[D \mid H_{1} \text { and } X\right]=1 / 2 ; P\left[D \mid H_{2} \text { and } X\right]=1 ; P\left[D \mid H_{3} \text { and } X\right]=0
$$

TABLE 1.4 The Monty Hall problem: standard assumptions

| Hypothesis <br> $H$ | Prior <br> probability <br> $P[H \mid X]$ | Sampling <br> probability <br> $P[D \mid H$ and $X]$ | Pathway <br> probability <br> $P[H \mid X] P[D \mid H$ and $X]$ | Relative <br> proportion <br> $P[H \mid$ and $X]$ |
| :---: | :---: | :---: | :---: | :---: |
| $H_{1}($ door 1$)$ | $1 / 3$ | $1 / 2$ | $1 / 6$ | $1 / 3$ |
| $H_{2}$ (door 2$)$ | $1 / 3$ | 1 | $1 / 3$ | $2 / 3$ |
| $H_{3}($ door 3$)$ | $1 / 3$ | 0 | 0 | 0 |

Putting these into an inference table results in table 1.4. Our posterior probability for $H_{1}$ is the relative proportion $(1 / 6) /(1 / 6+1 / 3)$, or $1 / 3$, with the remaining probability of $2 / 3$ going to $H_{2}$. Thus, switching doors is definitely to our advantage, doubling our chance of winning.

But let's see what difference a slight change to some of the standard assumptions could make. For example, we could imagine knowing that the host has an extreme hatred for door 3 and will open it only if absolutely necessary not to reveal the prize. Under that assumption, we have the probability for $D$ under $H_{1}$ equal to 0 , since in that case the host could have opened door 2 instead. And we see the only possibility remaining is door 2, so we should definitely switch!

On the other hand, maybe the host loves door 3 and will always open it if given the chance. Under that assumption, we have the probability for $D$ under $H_{1}$ equal to 1 , and the resulting inference table is table 1.5. This time our posterior probability for $H_{1}$ is $(1 / 3) /(2 / 3)=1 / 2$, so switching doesn't matter!

TABLE 1.5 The Monty Hall problem: the host loves door 3

| Hypothesis <br> $H$ | Prior <br> probability <br> $P[H \mid X]$ | Sampling <br> probability <br> $P[D \mid H$ and $X]$ | Pathway <br> probability <br> $P[H \mid X] P[D \mid H$ and $X]$ | Relative <br> proportion <br> $P[H \mid D$ and $X]$ |
| :---: | :---: | :---: | :---: | :---: |
| $H_{1}($ door 1$)$ | $1 / 3$ | 1 | $1 / 3$ | $1 / 2$ |
| $H_{2}$ (door 2$)$ | $1 / 3$ | 1 | $1 / 3$ | $1 / 2$ |
| $H_{3}($ door 3$)$ | $1 / 3$ | 0 | 0 | 0 |

It all hinges on what we assume about the host's feelings about door 3, which we could dial anywhere from absolute hatred to absolute fondness and get a range of answers from "You must switch to have any chance of winning" to "It doesn't matter at all whether you switch."

Returning to the assumption about the host necessarily offering the choice to switch, we could, of course, imagine this is not the case. Suppose the host is malicious and wants us to lose. Since he knows where the car is, he could decide to offer the switch only if we chose correctly in the first place. If we are wrong, he simply opens our choice of door and moves on to the next contestant. Under those assumptions, our observation is now incompatible with assumption $\mathrm{H}_{2}$, so the posterior probability for $H_{1}$ is 1 (it's the only case consistent with what we've seen). As a result, switching reduces our chance to 0 !

In fact, this turns out to be pretty close to the behavior of Monty Hall (who understood the problem and its solution). In an interview in the New York Times years later, he revealed that the rules of the show actually did not force him to offer a switch at all, and he was free to do whatever he thought would most heighten the drama of the show. As he put it, "If the host is required to open a door all the time and offer you a switch, then you should take the switch. But if he has the choice whether to allow a switch or not, beware. Caveat emptor. It all depends on his mood." 48

We have one final variant to consider: What if the host doesn't know where the car is? (In this version, we're explicitly told otherwise, but this part is often left out.) It may even be the case that he usually knows but happened to forget this one time. Maybe we see him give a heavy sigh of relief when door 3 is opened and the car isn't there. Under any of these assumptions, we give the probability assignments

$$
P\left[D \mid H_{1} \text { and } X\right]=P\left[D \mid H_{2} \text { and } X\right]=1 / 2
$$

because our observation includes the fact door 3 was opened. Even assuming $\mathrm{H}_{2}$, it could just as well have been door 2 that got opened; by luck, it happened not to be. The resulting inference table is table 1.6. And our posterior probability assignment is $1 / 2$. So, once again, switching adds nothing! In the original problem, it is the host's knowledge of what to do if the car is behind door 2 that allows him to add information and shift the balance of probabilities. Confusing our ignorance for the host's is what led to the intuitive-but wrong-answer to the problem.

But it all depends on what we assume.

TABLE 1.6 The Monty Hall problem: the ignorant or lucky host

| Hypothesis <br> $H$ | Prior <br> probability <br> $P[H \mid X]$ | Sampling <br> probability <br> $P[D \mid H$ and $X]$ | Pathway <br> probability <br> $P[H \mid X] P[D \mid H$ and $X]$ | Relative <br> proportion <br> $P[H \mid D$ and $X]$ |
| :---: | :---: | :---: | :---: | :---: |
| $H_{1}($ door 1$)$ | $1 / 3$ | $1 / 2$ | $1 / 6$ | $1 / 2$ |
| $H_{2}$ (door 2$)$ | $1 / 3$ | $1 / 2$ | $1 / 6$ | $1 / 2$ |
| $H_{3}($ door 3$)$ | $1 / 3$ | 0 | 0 | 0 |

## WHAT PROBABILITY ISN'T

Note at no point while solving either the Boy or Girl Paradox or the Monty Hall Problem did we make reference to frequencies or proportions of some hypothetical population. Most standard solutions for the Boy or Girl Paradox will involve imagining "sampling a random family from among those with two children" or an even more grotesque idea like "selecting from an urn full of children." Some, like Gardner himself, have argued that the question as stated is ambiguous because of its "failure to specify the randomizing procedure," 49 whatever that means. There's no need for any such specification. Where in the problem does it say anything about something being chosen at random?

Similarly, solutions to the Monty Hall Problem often involve simulating results, using a random number generator, to show that, over the long run, a strategy of switching leads to winning the car about two-thirds of the time. (This was how Erdős eventually became convinced.) These simulations will produce the "right" frequencies, though, only if the behavior of the virtual host is coded up to match the assumptions we've made-in particular, choosing an available door not hiding the car at random and always offering the contestant the choice to switch. So, if those assumptions are inconsistent with our actual state of knowledge, the simulation proves nothing.

Probability as logic has no need for such artificialities. Using Bayesian logical analysis, we can analyze each problem as though it is a single occurrence, with no need to think about some hypothetical random sampling procedure delivering us this information or some long-run sequence of events. We simply condition on what we know or are told is true, and we process the available information into a probabilistic inference. That inference will necessarily involve some
assumptions, sometimes complex ones about the people involved-especially if our observation includes someone doing something or telling us something rather than just some propositional fact. But first we need to slow down our thinking and carefully inspect all the information we're given and the assumptions we're willing to stipulate to finish the problem. Those assumptions might be wrong. Maybe Monty Hall has more fondness for door 3 than we assumed, and maybe Mr. Smith is equally proud of his son and his daughter, and maybe there never were two children to begin with, and maybe the game show is rigged against us.

Jaynes's essential point bears repeating: probability is about information. It comes from what we observe, what we are given, and what we hold to be true. We should want our assumptions to be true, and, indeed, if we are able to conceive of alternatives, probability as logic tells us how we should go about testing those alternatives based on observed fact, how surprised we should be to see one kind of observation or another, and how much evidence this provides in support of one hypothesis or another. But the only valid tools for processing that information, if we hold to the general rules for consistent reasoning given by Cox and Jaynes, are the rules of probability-specifically, Bayes' theorem. Cox's theorem shows that these rules depend on something more fundamental than ideas of frequency and proportion. In fact, they are derivable just from a weak assumption that our probabilistic reasoning process is logically consistent. Any form of reasoning that is "non-Bayesian" violates these conditions and is necessarily illogical.

These example brainteasers reveal the power of the probability-as-logic interpretation and show the steps required to assign probabilities in any problem of inference. The consequence for skipping any of the steps in these problems is harmless (other than some mild embarrassment), but in the real world, it often is not. In the next chapter, we will see several very real instances of people's lives being ruined because of a misuse of probabilistic inference.

