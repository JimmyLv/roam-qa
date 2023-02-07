**Abstract**. Roam is an online workspace for organizing and evaluating knowledge. The system is built on a directed graph, which frees it from the constraints of the classic file tree. Users can remix and connect ideas in multiple overlapping hierarchies, with each unit of information becoming a node in a dynamic network. Any given node can occupy multiple positions simultaneously, convey information through defined relationships, and populate changes throughout the graph. With weightings assigned to the strength of relationships between nodes, Roam also becomes a tool for Bayesian inference and decision making. The ultimate goal is to extend the system to collaborative reasoning, allowing groups to build shared mental maps and make faster and better-informed decisions.

**1.    Introduction**

We are experiencing an unprecedented explosion of knowledge. Every day, 2700 books are published in the United States alone, 6850 scientific papers are authored, more than 2 million blog posts go live, and 294 billion emails fly back and forth. The amount of total data produced with every rotation of the Earth would fill a stack of books stretching to the moon and back. [1](((u-XvVlybt))) While this exponential growth presents enormous opportunities for individuals and society at large, neither the human brain nor current technologies are equipped to harness it to its full potential.

**2.   Current approaches to knowledge management**

Humans are poorly adapted to the Information Age, which has arisen only in the last ~0.02% of our evolutionary history. While the brain does have a remarkable capacity for raw storage, probably in the range of several petabytes,[2](((PWlZyEjRU))) it is infamously fallible in processing information. Memory retrieval is lossy and unreliable, while many of our hardwired cognitive biases and heuristics misfire in the modern world, distorting our perception, judgement and decision-making ability. The plasticity of the brain enables it to rewire itself with new connections, but even this is a ‘use it or lose it’ feature, causing neglected neural pathways to atrophy.

Many technologies for organizing knowledge outside of the brain have arisen in response to these limitations. Physical books and journals proliferated after the invention of the Gutenberg Press, and have since been partially supplanted by word processors, websites, blogs, forums, wikis, and software applications.

While we are presented with a plethora of choices for organizing knowledge, almost every technology follows the same basic ‘file cabinet’ format: A unit of knowledge is saved to a certain file path, which places it within a taxonomy of folders, chapters or categories. Tags may be applied when an item relates to many things, but each file is generally only stored within one nested hierarchy. To access the information, the user must remember where they stored the file, what they tagged it with, or use a search function to locate it.

Related Twitter Thread

https://twitter.com/Conaw/status/1099181050045952006

**3.   Problems with the file cabinet approach**

In some regards, current technologies remain vastly inferior to the human brain. If each neuron only held a single ‘unit’ of memory in this manner, our brains would quickly fill to overflowing. Instead, information is conveyed in the connections between neurons and neural networks, so a common idea can be made available across the entire brain; the concept of a blue sky might be used in countless seemingly discrete memories of time spent outdoors. This efficiency helps to explain why a computer requires several million times more energy to perform the same tasks as a human brain (which runs on about as much power as a dim light bulb).[3](((j6_rKU-PG)))

Unlike the brain, the file cabinet approach makes it difficult or impossible to remix or reuse the same piece of information. Each time a change is made to any given file, it has to be tracked down and updated in every location in which it exists. This leads to redundancy, with a cluttering of near-identical ideas, and significant work any time a system-wide change is required.

Current solutions also lack interconnectivity. Many files are divorced from context; cast into a drawer, rather than methodically fitted into a broader framework of knowledge. Knowledge trees can create pseudo-relationships between files nested within a given hierarchy, but these are not explicit, and can only describe a vertical ‘parent and child’ taxonomy. Some tools, such as web pages and wikis, also allow for orthogonal linking between related files, but this takes place in an ad hoc fashion, and again, there is no ability to explicitly define relationships.

**4.	Knowledge graphs as nodal networks **

Large-scale collaboration requires a more flexible data structure than the classic file tree. Roam is built on a knowledge graph that maps all possible relationships, with ‘smart’ links between defined concepts. Users can connect similar ideas in multiple overlapping hierarchies, remix them without overwriting the original context, and selectively share parts of the graph with others to collaborate on specific sub-questions.

If current tools resemble filing cabinets, Roam is more akin to the nodal networks in telecommunications, or the neurons in the human brain. Rather than existing in a vacuum, each note or file becomes a node in an interconnected graph of ideas. A single node may simultaneously hold positions in several different sequences, hierarchies or file paths, and can ‘talk’ to other nodes, communicating information back and forth about the nature of each relationship. The network is dynamic, so updates and revisions are populated across the entire graph simultaneously. Individual nodes or branches within the network can be forked as required, allowing a new pathway to deviate without changing the original meaning.

At the simplest level, Roam’s structure makes it inherently easier to store, recall, and cross-reference ideas. This is the primary proposition for students, writers, self-directed learners, and users of existing note-taking apps.  

For power users, the knowledge graph also unlocks applications in logic and reasoning, Bayesian inference and decision-making, modelling complex problems, and collaborative research.

These features are explored in Chapters 5 - 8, along with potential use cases for the technology. 

**5.	Dependency graphs and logical reasoning**

Everything from peer-reviewed research papers to the opinion pages of a newspaper are based on formulating arguments that support a certain premise, along the lines of the following: 

If A is true, then B is true.

If C and D are both true, then A is true.

C and D are true.

Therefore, B is true.

Example:: [[Precise Links]]

{{embed:((PWRiHAsEv)) }}



Often, C and D will be supported by links to external articles, where they are conclusions reached by larger arguments based on combining other premises. Unfortunately, the structure of the argument is only implied by the prose. Rarely are the relationships between arguments and pieces of evidence explicitly laid out, except perhaps in the notes of the author investigating the claims.

Roam allows individual researchers or writers to organize all the claims they wish to make across a number of different projects. It also creates opportunities for large-scale interdisciplinary research projects. When teams of interested collaborators have an agreed-upon structure for formatting arguments and counterarguments, it is possible to create expandable user interfaces which “bubble up” insight from claims which require expertise, to ones that are more easily understood by laypersons.

The ambiguity of natural language derails many discussions. Unless [[terms]] are clearly defined from the outset, any form of argument is futile, and will often end up entrenching the initial positions of the interlocutors.

Example A

Alice:  "A tree falling in a deserted forest makes a sound."

Bob:  "A tree falling in a deserted forest does not make a sound."

Example B

Alice:  "A tree falling in a deserted forest [generates acoustic vibrations]."

Bob:  "A tree falling in a deserted forest does not [generate auditory experiences]." [4](((T8k78DDAe)))

While these positions are contradictory as expressed in Example A, simply defining the term ‘sound’ reveals the underlying beliefs are entirely compatible. 

The ability to use clearly defined sets within a dependency graph helps to resolve ambiguity, reducing the chances of participants talking at cross-purposes, or deliberate “motte-and-bailey” style strategic equivocation. [5](((MtGChSUvh)))

Besides reasoning and argument, dependency graphs have applications in education, self-directed learning, and general decision-making. Even a very complicated project can be traced backwards to a number of smaller [[task]]s. The user can see the tradeoffs involved in each pathway, map out which route is the fastest, and which path might bring them closer to other interesting goals. As the student marks their progress, they can discover new projects and pathways which make use of the skills they have acquired.

The problems of prose apply even in the domain of mathematical proofs, see Lamport’s [[How to write a 21st Century Proof]]”

**6.	Untangling complexity**

**6.1	Nonlinear causality**

Simple problems often follow a straightforward causal path. When a patient has a range of symptoms strongly associated with the flu, the doctor might conclude from the observable variables that there is one invisible variable - the influenza virus. Treat that latent variable, and the symptoms disappear. 

Scott Alexander observes that his peers in psychiatry similarly try to attribute a collection of linked symptoms to a latent variable; for example, depression. [6](((36qeTMgmO))) However, the symptoms ‘caused’ by depression - e.g. sleep disturbance, fatigue, guilt - can also have a causal effect on one another, and on the disorder itself. This complex web of relationships, which may include feedback loops, does not follow a path of linear causality. For complicated problems of this nature, nodal networks are a much more accurate model:

A model of major depression (MD) and generalised anxiety disorder (GAD) by Nuijten, Deserno, Cramer, and Borsboom.[7](((rC_nGuzjf))) The disorders roughly map onto clusters of symptoms that are often found together and reinforce one another, but there is no clear ‘bright line’ between the conditions.

Even at face value, a nodal network provides a visual aid to problem-solving - a bird’s eye view of the connections between various elements. This may help to identify patterns or clusters which may be counterintuitive or entirely invisible when each piece of the puzzle is examined at the object level.

**6.2	Bayesian reasoning**

Applying Bayesian reasoning to the knowledge graph makes it a powerful tool for estimating probabilities, testing hypotheses, and making decisions. Bayes’ Theorem is a law of probability that tells us how much we should change our minds about something when we learn a new fact or acquire new evidence. The theorem is stated in the following equation:

        $$P(A|B) =  {P(B|A) P(A) \over P(B)}$$ 


where A is the proposition of interest, B is the observed evidence, P(A) and P(B) are prior probabilities, and P(A|B) is the posterior probability of A.

Suppose a doctor has a patient who is worried about carrying a latent disease, because he belongs to an at-risk group. This is the ‘proposition of interest’ on the left side of the equation. Prior data suggests 4% of the general population are carriers, so $$P(A) = 0.04$$. B is the observed evidence, which is that 32% of the general population are members of the at-risk group. $$P(B) = 0.32$$. The doctor knows that among patients who do carry the disease, 80% belong to the at-risk group: $$B|A = 0.8$$.

The doctor applies Bayes’ theorem:

$$P(A|B) = (0.8 * 0.04)/0.32$$

$$P(A|B) = 0.1$$

Her patient only has a one in 10 chance of being a carrier - which might be less than expected, given that almost all carriers are members of the at-risk group. 

While this is a simple calculation, the strength of Bayesian reasoning is that it breaks down seemingly insurmountable problems into small pieces. Even where no data are available, successive layers of estimates can still provide useful refinements to the confidence levels of various outcomes. By incorporating this framework into the defined relationships between nodes, revisions to the weightings at any point in the network will automatically populate throughout the knowledge graph.

Bayesian probability also provides a framework for decision-making. By estimating the costs and tradeoffs of various options, users can calculate which pathway provides the highest expected value. Again, the quality of the decisions can be refined by successive layers of evidence for and against, even when the weightings are simple estimates of personal preference. An evaluation matrix allows someone to integrate a great deal of information into the final decision, rather than defaulting to simple heuristics.

{{[[TODO]]}} [Example [[Diagrams]] of decision tree/matrix] 

**7.	Optimising for **[[Serendipity]]

Just as humans are incapable of generating random numbers, we struggle to consciously generate random ideas - to the point where actively trying to ‘think differently’ often seems to only further calcify existing patterns. Instead of attempting to brute-force creativity, the brain must be confronted with novel stimuli in order to reorganize its perception. Exposure to a certain amount of random ‘noise’ - drugs, dreams, meditation, Tarot readings, mistakes - can jolt thoughts out of well-tracked grooves and into entirely new areas of idea-space. Typically these insights occur at the juncture of two or more seemingly unrelated fields, concepts, or images. 

The interconnectivity of the Roam knowledge graph constantly creates opportunities for [[Serendipity]] to blossom. Each node in the network can be viewed in several graphical displays, allowing users to see related ideas, scan up and down the vertical hierarchy, examine nearby clusters of nodes, and observe patterns. 

The Roam search function can be calibrated to include as much or as little ‘noise’ as the user desires. While looking for a specific passage or note, search is narrow enough to find exactly what the user has in mind. However, it can also be broadened out for ‘fishing trips’ aimed at surfacing categories of ideas. Some search results will consist of notes that the user might otherwise have forgotten about, some will be noise, and others will spark ideas the user didn’t even know they were looking for.

The synthesis and cross-pollination of ideas from diverse fields presents low-hanging fruit for both individuals and society. The investment of time and effort required to become a specialist quickly runs into a point of diminishing returns. By contrast, accumulating a ‘talent stack’ of dilettante-level knowledge or skills can unlock insights and opportunities that have not been capitalised on by experts with a narrower focus.

Highly specialised knowledge remains essential for opening new frontiers. However, an interdisciplinary approach is often required to solve the increasingly complex problems faced by scientists, technologists, and policymakers.

**8.    Collaborative problem-solving**

While the individual use case for Roam stands on its own merits, the ultimate goal is to create a platform for collaborative research and learning. Current protocols are bound by the assumption of necessary consensus. The flexibility of a curated knowledge graph allows for a more pluralistic approach, with the ability to weight conflicting opinions and separate signal from noise without resorting to either autocracy or democracy. 

8.1	**Finding signal in the noise**

As the frequency of information increases, the world becomes noisier and noisier. Deliberate exposure to noise is a useful strategy in specific contexts, as described in Chapter 7,  but otherwise obscures meaning. [8](((urKnXjnSR))) Given we have a propensity for imposing stories and explanations onto randomness - the narrative fallacy - it is becoming increasingly difficult to separate out genuine signal from noise. 

Assume a trend has a signal-to-noise ratio of 1:1 on an annual basis (50% of the data are meaningful, 50% are random). Observing the same data on a daily basis, the composition changes to 95% noise, 5% signal. Observing the data hourly (as news hounds and market junkies do), and it becomes 99.5% random - which is to say, two hundred times more noise than signal.[9](((_eOgBulZd)))

Institutions entrusted with interpreting the data include the media, academia, and legislature. Some agents within these institutions deliberately obscure the truth, as demonstrated by ‘fake news’, p-hacking, and politicking. While actively malicious behaviour is the exception, even the best-intentioned reporters, researchers and analysts are not immune to being fooled by randomness.

For most people, the problem of sorting signal from noise therefore involves finding trustworthy and accurate secondary sources of information. This difficult [[task]] is often frustrated by gated scientific journals, as well as search engine algorithms increasingly gamed by SEO-savvy content marketers.

8.2	**Redundancy**

Navigating a vast sea of information creates massive redundancy. Most people labour away at problems that have already been solved a million times over. Those who tackle unsolved problems often do so in silos, unaware of each other’s existence. All the pieces of any given puzzle may be present, but no one individual or group holds them all. The wheel is reinvented over and over again, in endless forums and comments sections and web pages and books that burst into existence and fade just as quickly to obscurity.

The goal of Roam is to enable systematic curation and collaboration on a large scale. Users will be able to selectively share parts of their graphs publicly, or with circles of peers and colleagues. In turn, they will be able to follow the work of persons they trust, whether they be domain experts or enthusiastic amateurs. Those looking to acquire specific knowledge can turn immediately to trusted sources, and set alerts to receive updates about new pieces of information pertaining to an area of interest.

8.3	**Dispensing with necessary consensus**

Almost every medium today presents knowledge as though it were the last word; assuming both a necessary consensus and an uncomposable page. Wikipedia is one of the great wonders of the Internet age, but it makes both of these mistakes. There can only be one article on any subject for any given language, and the only connection between pages is through links, with no article "built" off another.

By way of contrast, consider Github: Libraries are built on other libraries, and functions are built from other functions. Developers build tools that others can build upon to build ever more impressive tools. Most of the modern web is built on open-source technologies, which would not have been possible if programmers followed the old protocols for intellectual collaboration.

Many problems can be solved by writing code, but natural language is still the way we determine which problems are worth solving. Natural language is how we explain the world to one another, and communicate our models of reality. It is the language of education. It is the language of decision-making. That language needs a toolchain for collaboration that is just as good as the one for managing code.

8.4	**Against autocracy; against democracy**

The problem of necessary consensus is resolved by individuals or groups assembling their own graph of inferences, based on premises or data curated from their trusted networks. However, collaboration still requires a mechanism for evaluating which ideas are best. In the same way that individuals assign weightings to their personal predictions and decisions,  groups must be able to ‘vote’ on the merits of any given idea, premise, or piece of evidence. There are various options for how these collective weightings might be calibrated, some of which are briefly described below.

a) **Wisdom of crowds**

A diverse collection of people can make certain decisions and predictions much better than any given individual: The great statistician Francis Galton was stunned to find that 800 people guessing the weight of an ox at a country fair returned an average that was just one pound shy of the correct figure of 1198 pounds. 

In other situations, the opinion of the crowd bears little relationship to objective reality. By definition, the tyranny of the majority will quash any position that is unpopular, regardless of whether it is true. Often, domain-specific knowledge may be required; for example, someone who has not studied free will would only be adding noise by ‘voting’ a preference for compatibilism, hard determinism, or libertarianism. 

Simple popularity contests do not always move us closer to the truth, but they are useful in that they tell us what we believe. This data could potentially be broken down by demographic to demonstrate how different groups perceive reality, and possibly alert users to biases amongst their own in-groups.

b) **Believability scores**

Hedge fund manager Ray Dalio pioneered a decision-making system at Bridgewater Associates that is much closer to epistocracy than democracy: The opinions of more “believable” people, who have repeatedly proven their grasp of a given topic or trait, hold more weight than those with lower believability scores. There is nothing to stop Dalio being overruled by his most junior employees, as long are they are consistently more right than he is. Implementing a similar system in Roam would necessitate the ability to track performance, perhaps by how much original content a user has contributed to the graph with broad support, or how well-calibrated their predictions are.

c) **Prediction markets**

When people succumb to peer pressure and other biases, do not have enough specialist knowledge, or deliberately make false predictions, the ‘wisdom of the crowd’ can end up being very wrong.

The insight behind prediction markets is that participants can be incentivised to profit from any such mistakes. Wherever someone believes the consensus is wrong, they can stake money on it, and move the probability back to a better informed position. Insider information is not only permitted, but welcomed. In this way, vast amounts of information can be synthesised into one constantly updated data point, which is often remarkably accurate.

The uptake and growth of prediction markets has been dampened by regulatory issues, but possible workarounds include a non-fiat token, or reputation-linked points system.

**9.    Conclusion**

The project of human knowledge, as it stands today, is a vast ocean of ephemeral and fragmented information and ideas, much of it inaccurate, some of it malicious, with the best sources either restricted by gatekeepers, or near-impossible to locate. The volume of information is growing exponentially, which promises enormous opportunities if the underlying coordination problems can be resolved.

Clearly a fundamentally different approach is required. The Roam vision for human knowledge is a collective, open-source intelligence, constantly rearranging, iterating and evolving in the pursuit of truth.  Each of us would become a node within this collective intelligence, forging links and creating networks, sharing the very best each has to offer, improving ourselves even as we improve others, and advancing the interests of humanity as a whole.

About Roam

Roam was founded by Conor White-Sullivan and Joshua Brown. Conor has been working on tools for collective intelligence for more than nine years, founding the online town common Localocracy (acquired by AOL in 2011) then leading R&D for Huffington Post following the acquisition. Conor and Josh met at 42.us.org, a tuition-free coding university, where Josh placed in the top five of the first 1000 cadets to enter the US program during the month-long application exam. This white paper was co-authored by business journalist Richard Meadows, whose trial of early prototypes led him to become the first investor in Roam.

The Roam stack:

React

Clojure and Clojurescript

Datalog

Contact Conor at cwhitesullivan@gmail.com with any enquiries.

Notes and references

[1] At least 2.5 quintillion bytes of information are produced every day, which is about the same amount as was produced during the entire year of 2002. 

[2] Scientific American: New Estimate Boosts the Human Brain's Memory Capacity 10-Fold.

[3] Microelectronics pioneer Carver Mead, who coined the term Moore’s Law, correctly predicted in 1990 that present-day computers would use ten million times more energy for a single instruction than the brain uses for a synaptic activation.

[4] This example is adapted from the Less Wrong sequence 37 Ways Words Can be Wrong.

[5] Motte-and-bailey refers to arguing an easy-to-defend and often common-sense statement (the motte), in order to ward off critics from a hard-to-defend and more controversial statement (the bailey). The term was popularised by Scott Alexander, and explained in All in All, Another Brick in the Motte.

[6] Slate Star Codex: Mental disorders as networks.

[7] Michèle B. Nuijten, Marie K. Deserno, Angélique O. J. Cramer, Denny Borsboom: An introduction and overview of a network approach to psychopathology.

[8] As Carl Sagan observed, while more data is broadcast in TV programs every day than the combined written works of all of history, "not all bits have equal value".

[9]  This example comes from Nassim Taleb’s Antifragile.

Further Reading

Daniel Kahneman, Thinking, Fast and Slow

Robin Hanson, Could Gambling Save Science?

[[Ray Dalio]], [[Principles]]

H Van Dyke Paranuk, Don’t Link Me In: Set Based Hypermedia for Taxonomic Reasoning

[[Michael Nielsen]], Reinventing Discovery: The New Era of Networked Science

Richards J Heuer The Psychology of Intelligence Analysis

Leslie Lamport: [[How to write a 21st Century Proof]]

Douglas Engelbart, [[Augmenting the Human Intellect: A Conceptual Framework]]

About this Paper

We wrote this White Paper in Winter of 2017/2018, and while it still reflects much of our vision for the tool, some of the features -- particularly related to [[Bayesian Reasoning]], [[Argument Analysis]], and [[Prediction Markets]] we found to be in-fact much lower priority for the researchers and decision makers whose thinking we aim to assist -- and risked making the tool too complex for the more significant use cases.  If you are interested in using Roam for more formal Quantitative Reasoning or building out formal models of belief networks, or if you are excited about ideas in this paper which you do not see a way to do currently within Roam, please contact us.  

