---
author: Soham Ghosh
#categories:
#- Theme Features
date: "2021-09-05"
draft: false
excerpt:
title: Nonconglomerability and the Law of Total Probability
---

This explores the unsung sector of probability : **"Nonconglomerability"** and its effects on conditional probability. This also emphasizes the idea of how important is the idea countable additivity or extending finite additivity to infinite sets.

> *“I believe that we do not know anything for certain, but everything probably.”~ Christiaan Huygens*

One week into conditional probability, it's time to get our hands dirty with the **Law of Total Probability** and paradoxes which have emerged out of it.Let's be formal enough to state the law first.

### The Law of Total Probability

Adorably called **LOTP**, it is one of the cardinal results in Conditional Probability.

Suppose the events \\(A_1, A_2, ..., A_k\\) are a partition (mutually exclusive and exhaustive) of the event space and let **H** be any arbitrary event of the event space then it states that \\(\mathbb{P}(H) = \mathbb{P}(H|A_1)\mathbb{P}(A_1) + \mathbb{P}(H|A_2)\mathbb{P}(A_2) + ... + \mathbb{P}(H|A_k)\mathbb{P}(A_k)\\).

![](P1.png)

The day to day event I always relate to while recalling this law is that Suppose you have a thin glass block placed on a table and accidentally some water has been spilled on it. A part of this water has been trapped in between the surface of the table and the glass. If you look at this from above, you will see a puddle of water almost circular,trapped within the rectangular block. This puddle is actually our arbitrary event **H** and our block the event space. How can you get the partitions? Any wild guesses? Well, drop a hard stone on the glass and it cracks, or even if you have strong arms and like fantasizing about hurting your knuckles, you can do it too :P. The cracks partition the sample space into various segments and there is water trapped in each of them. There you go!

As we have stressed already, from a false proposition, or from a fallacious argument that leads to a false proposition - all propositions true and false, may be deduced.But this is just the danger;if fallacious reasoning always led to absurd conclusions,it would be found out at once and corrected.But once an easy , shortcut mode of reasoning has led to a few correct results, almost everybody accepts it; those who try to warn against it are generally not listened to.

When a fallacy reaches this stage, it takes on a life of its own and develops very effective defenses for self preservation in the face of all criticisms.Here is one such instance.

### Nonconglomerability

If \\(C_1, C_2, ..., C_n\\) denote a finite set of mutually exclusive, exhaustive propositions on prior information **I** , then for any proposition **A**, we have :

$$\mathbb{P}(A|I) = \sum_{i=1}^{n}\mathbb{P}(A \cap C_i|I) = \sum_{i=1}^{n}\mathbb{P}(A|C_{i}I)\mathbb{P}(C_i|I)$$

As you all seen in the previous blog post, the prior probability \\(\mathbb{P}(A|I)\\) is written as a weighted average of the conditional probabilities \\(\mathbb{P}(A|C_{i}I)\\).

Now, it is an elementary result that the weighted mean of a set of real numbers cannot lie outside the range spanned by those numbers, i.e., if \\(L \leq \\(\mathbb{P}(A|C_{i}I)\\) \leq U\\); then necessarily \\(L \leq \\(\mathbb{P}(A|I)\\) \leq U\\).

**De Finetti** (1972) called this property as **"conglomerability"** of the partition \\({C_i}\\).

Obviously, non-conglomerability cannot arise from a correct application of the rules of probability theory on finite sets. It cannot, therefore occur in an infinite set which is approached as a well defined limit of a sequence of finite sets.

Yet, nonconglomerability has become a minor industry, with a large and growing literature.There are writers who believe that it is a real phenomenon, and that they are proving theorems about the circumstances in which it occurs, which are important for the foundations of probability theory. Nonconglomerability has become, quite literally, institutionalized in our literature and taught as truth.

Let us examine some case where **"nonconglomerability"** has been claimed to be true.

### Rectangular Array

This particular example by the famous trio **Kadane**, **Schevish** and **Seidenfeld** (1986).

We start from a 2 dimensional **(M×N)** set of probabilities :

$$p(i,j), 1 \leq i \leq M; 1 \leq j \leq N$$

The **sample space** is a **rectangular array** of **MN** points in the first quadrant. It will suffice to take some prior information **I** for which these probabilities are uniform :

$$p(i,j) = \frac{1}{MN}$$

Let us define the event **A : i < j **.

Therefore, \\(\mathbb{P}(A|I)\\) can be found by direct counting and in fact it is given by :

$$\mathbb{P}(A|I) = \begin{cases} 
  \frac{2N - M - 1}{2N}, M \leq N\\
  \frac{N - 1}{2M}, N \leq M\\
\end{cases}$$


