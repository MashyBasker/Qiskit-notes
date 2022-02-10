# Classical Probability

When we see from the perspective of coin toss, we know from our school days that it'll be 50%. 

The best way way to visualise this is by making probability trees.

![Classical probability](https://mammothmemory.net/images/user/base/Maths/Statistics%20and%20probability/Outcomes%20and%20Expected%20Frequency/probability-tree-for-tossing-a-coin-twice.c951adc.jpg)

We have 1/2 probability of getting heads or tails when we start from either.

This probability remains same no matter how many times we perform the toss (we will see very soon that this is not the case at all times!)

Things seem pretty good for now.

### ENTER QUANTUM!!
<br>

# Quantum probability

Quantum coins are a special creation of years of hardwork, cool physics and scary (persepctive) maths.

### Quantum Coins
---
Quantum coins aren't really *coins* in our usual sense. Firstly they're called qubits.

Instead of having heads and tails they remain in the state of 0's and 1's.

When peforming a qubit (quantum coin will be referred to as qubit here after) toss once we get the good 'ol 50% probability of getting 0 or 1 like we are used to.


![quantum toss](https://qiskit.org/textbook/images/whatis/whatis7.png)

So far so good.

But when we do a double qubit toss, we see some unexpected behaviour.

Let's say we perform the qubit toss when the initial state was 0, after the second time we see that P(0) is 100 % whereas p(1) is 0 %. This is unnatural, this shouldn't happen right? But no matter how many times we perform the double qubit toss, the probablity of the state we started from always ends being 100 %.

Our probability model has failed us, this is the same bewilderment that the physicists felt in the early 20-th century.

This discovery led to the development of The Quantum Model!

## *The Quantum Model*
---
To say in simple terms, quantum theory is probability theory with negative numbers. 

But we now that probabilities cannot be negative.
Scientists figured out a cool trick to get around the fact that probabilites cannot be negative and the sum of probabilities should be 1 ; instead of taking the direct probability, we take their squares. This squared quantity is called the *amplitude*.

Now the probability of a quantum coin with intial state of 0 will look like this,
<br>

![quantum model](https://qiskit.org/textbook/images/whatis/whatis9.png)

We see that during the first toss, the amplitudes are assigned equally to both the states 0 and 1. The square of these amplitudes give us the probabilities P(0) = 1/2 and P(1) = 1/2.

Now where did we get the value 1/$\sqrt{2}$ ?

This is not an induction but a deduction. We took the values as 1/$\sqrt{2}$ because this the value that gives us the correct answer.

*There are actually better [mathematical explanations](https://quantumcomputing.stackexchange.com/questions/21257/why-in-quatum-coin-toss-when-starting-from-state-1-rangle-we-get-rangle) to this, but we will know about them later on*

Now we will see the quantum toss when the initial state is 1.

![toss1](https://qiskit.org/textbook/images/whatis/whatis10.png)

Here we see that the qubit toss with initial condition 1 gives use unequal amplitudes of 1/$\sqrt{2}$ and -1/$\sqrt{2}$ and squaring them gives us the known probabilities of 1/2 for both P(0) and P(1).

The negative sign is here because it gives the correct solution. This can also be considered as a consequence of [Hadamard Gate](https://www.quantum-inspire.com/kbase/hadamard/) (this is a slightly advanced topic and we will learn about it later on).

### Double Quantum Coin Toss
---
Putting the above two pieces together we can begin to understand the bizzare outcome of the double coin toss.

![double quantum toss](https://qiskit.org/textbook/images/whatis/whatis12.gif)

Here we see that the opposite sign probabilities of P(1) cancel out and the sum of the probabilites of P(0) add upto 1.

I don't completely understand this outcome myself, but I hope to do so as I keep learning more.

---
### SOME EXTRA LINKS :
- [Qiskit Textbook](https://qiskit.org/textbook/what-is-quantum.html#Going-Further)
- [Quantum Computing Model](https://csis.pace.edu/ctappert/cs837-21spring/QC-evans.pdf)

---
