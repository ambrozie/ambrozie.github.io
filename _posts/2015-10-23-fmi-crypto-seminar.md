---
layout: post
title: FMI Crypto Seminar
published: true
---


Recently I've attended the first meeting of what I hope will turn into the first fully fledged cryptography seminar in Romania.

Before moving on, I'd like to take the time to mention the event organizer, [FMI](http://fmi.unibuc.ro/) Crypto Group, and give them a big and well-deserved thank you for their initiative.

<!-- more -->

Now that I've set the scene, I will first talk about this first meeting and and how it went.

### What the First Meeting Was About

This meeting's lecture was an introduction to lattice based encryption by [Dragos Alin Rotaru](https://twitter.com/dragosrotaru). His affiliation is [Bitdefender Romania](http://www.bitdefender.ro/) (I was pleasantly surprised to find out they invest in theoretical research) and [University of Bucharest](http://www.unibuc.ro/). I first met Alin while attending the [Summer School on Secure and Trustworthy Computing](http://summerschool.trust.cased.de/) so I was eager to see him lecture.

Probably now would be a good moment to mention that I've created a [repository](https://github.com/iambrosie/FMICryptoSeminar) for the purpose of collecting materials related to the seminar and you can already find Alin's slides there. I hope I'll be able to do this for future meetings as well.

I also think it's important to mention the audience amounted to roughly fifteen people and, as far as I could tell, consisted mostly out of [FMI](http://fmi.unibuc.ro/) students and [a few](http://ruxandraolimid.weebly.com/) [teachers](https://sites.google.com/site/adelageorgescucrypto/). I suspect there were some people from Bitdefender as well.

### How the Lecture Went

Before going ahead and relating my perception of how the lecture went, I'd first like to pause for a moment and note that my sole reason in writing this lies in trying to offer [constructive criticism](https://en.wikipedia.org/wiki/Constructive_criticism) for the purpose of increasing the overall experience for all parties involved.
 
Going back to the lecture, if I were to choose a single word to describe it, I would say it was succinct. I would have preferred a more rigorous approach (i.e. more maths - even introductory notions - when needed, more proofs - at least sketchy). Also, more references and links for the provided ones would be useful during the presentation, as well as when checking out the slides later. Pointers for further study would also be nice.

So now that I've pointed out the lecture's shortcomings, it's time for me to try and fix it. I will thus try to provide a list of resources for people interested in studying lattices and their usage in cryptography. Even though I have gathered these over time, I haven't studied them thoroughly so, as always, you should take this list with a grain of salt and decide for yourself what works and what doesn't. Also please ignore the order in which they're presented.  

### Lattices in Cryptography, Study Resources

[J.H. van de Pol - Lattice-based cryptography \[M.Sc. Thesis\]](http://www.cs.bris.ac.uk/pgrad/csjhvdp/files/ThesisJvdPol.pdf)

[Dong Pyo Chi and Jeong Woon Choi and Jeong San Kim and Taewan Kim - Lattice Based Cryptography for Beginners \[Lecture Notes\]](https://eprint.iacr.org/2015/938)

[Joseph H. Silverman - An Introduction to the Theory of Lattices and Applications to Cryptography \[Slides\]](http://www.math.brown.edu/~jhs/Presentations/WyomingLattices.pdf)

[2nd Bar-Ilan Winter School On Cryptography - Lattice-based Cryptography and Applications](http://crypto.biu.ac.il/2nd-biu-winter-school)

[Daniele Micciancio - Lattices Algorithms and Applications \[Course\]](http://cseweb.ucsd.edu/classes/sp14/cse206A-a/index.html)

[Oded Regev - Lattices in Computer Science \[Course\]](https://www.cims.nyu.edu/~regev/teaching/lattices_fall_2009/)

[Daniel Dadush, Oded Regev - Lattices, Convexity and Algorithms \[Course\]](http://cs.nyu.edu/courses/spring13/CSCI-GA.3033-013/index.html)

 
### So, What's Next?

What I hope for is more lectures and why not, larger audiences.    

*_Notes_  

During the lecture it was mentioned the fact that there are no cryptosystems which rely on the difficulty of the CVP (closest vector problem). I later found out this is not technically correct, as the [Goldreich–Goldwasser–Halevi (GGH) lattice-based cryptosystem](https://en.wikipedia.org/wiki/GGH_encryption_scheme) is an example of such a cryptosystem. I agree, the scheme is not secure considering the fact that Nguyen showed as early as 1999 that there is a flaw in the design of the scheme.

Also, during the lecture, I asked whether there are situations where the lattice dimension has an effect on the security of the schemes we wish to build. The consensus seemed to be no but I suspect this might not always be the case. As [this](https://eprint.iacr.org/2013/630.pdf) paper seems to suggest, lattice dimension in lattice-based schemes underlying Fully Homomorphic Encryption needs to be very large.
