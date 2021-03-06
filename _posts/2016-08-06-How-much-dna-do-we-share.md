---
layout: post
title:  "How much DNA do we share with our relatives? Inheritance and probabilities"
excerpt: "The One with all the DNA"
date:   2016-08-6 22:30:15
categories: [Probabilities]
comments: true
---
**Let's draw a hypothetic family tree.**

![dna1]({{site.url}}/img/dna1.jpg)

**First question: How much DNA do we share with our brother?**

We all studied at school that the 50% of our DNA comes from our mom, and the other 50% comes from our dad.

![dna2]({{site.url}}/img/dna2.jpg)

We also should know that we share the 50% of our DNA with our brothers and sisters. But this last thing is not so obvious.

**Why can't something like this happen?**

![dna3]({{site.url}}/img/dna3.jpg)

Why don't we have the part of our mom's DNA that our brother doesn't have?

It is possible to find the answer by using probabilities...

The number of genes of a human being is between 25 000 and 30 000. Let's assume that people have exactly 30 000 genes.

We inherit 15 000 genes from our mom, and another 15 000 genes from our dad.
Every gene of our parents have a 50% chance to pass to us.

Now is our brother's turn and we ask the following question: What is the chance to share one of the genes that our mom gave us with our brother?

The answer is simple. Our brother needs the 50% of our mom's DNA, from who we already took 15 000 genes.
Then, the chance for our brother to have one of our 15 000 genes from mom is 15000/30000.

![dna4]({{site.url}}/img/dna4.jpg)

This far, we already share with our brother half of the DNA our mom gave us, that's a 25% of all our genetic information.

We can do the same analysis with our dad's DNA, and we will have another 25% of shared DNA.

**What happen with our cousins? How much do we share with them?**

Mom and Sarah are sisters, they share the 50% of their DNA.
Our cousin Kenny is Sarah's son.

How much of his DNA does Kenny shares with our mom?

Kenny inherits the 50% of his DNA from Sarah, who shares the 50% of his DNA with mom. So, for every gen that Kenny inherits from Sarah, this gen has a 50% chance of being a gen that our mum also have. As result, the 50% of the genes that Kenny inherits from Sarah will be genes that he shares with our mom. That means that Kenny will share the 25% of his genes with our mom.

**So, how much DNA do we share with Kenny?**

![dna5]({{site.url}}/img/dna5.jpg)

Our mom have a 25% of Kenny's DNA. How much of this 25% can we inherit?
25% of 30 000 genes is 7500 genes.
Our chances are 7500/30000, that's 1/4. That means that 1/4 genes of the 50% that we inherit from our mom are genes that we share with Kenny.

![dna6]({{site.url}}/img/dna6.jpg)

1/4 of the 50% of our DNA is 15 000/4, 3750 genes, this represents 12,5% of our 30 000 genes.

So, that's it! We share the 12,5% of our genetic information with our cousins!

I wanted to solve this problem with any relative, so I wrote this [python script](https://github.com/abeagomez/genetic_calculator) where I can define a family tree and then ask for the percent of DNA shared between two family members.

