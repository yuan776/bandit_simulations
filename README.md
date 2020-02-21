# Bandit_simulations
Bandit algorithms simulations and analysis for online learning

This repo is part of my interest to learn more about optimisation for online learning algorithms which are heavily centerd on bandit theory. Based on what I understand, there are different types of bandit problems:
- __Multi-armed bandits:__ Bandits arms are inherently non-differentiable except for their inherent reward function. For multiple arm bandits, the objective is to determine the bandit with the highest reward function via online learning, which is a classic explore-versus-exploit problem.
- __Contextual bandits:__ Bandits with features (aka context) that interact differently with different actions. Different contextual features will require different actions to return the reward. This can be perceived as a classification problem: given input features aka context, what is the right classification of "actions" that will return high accuracy/reward?

This repo is segmented into both Python and R.
- Python: 
    - __Phase 1 MAB analysis:__ Comprises coding of certain Multi-Armed Bandit algorithms for experimentation. Largely based on the book ["Bandit Algorithms for Website Optimization"](https://www.oreilly.com/library/view/bandit-algorithms-for/9781449341565/) by John Myles White.
    - __Phase 2 CB analysis:__ Learning how to use the gold standard package for online learning `vowpal wabbit` for contextual bandits
- R: 
    - __Phase 3 MAB & CB analysis:__ Using R library package `contextual` that has a comprehensive ecosystem for different algorithm and policies

Phase 1 MAB analysis includes:
- [Epsilon Greedy](https://github.com/kfoofw/bandit_simulations/blob/master/python/analysis/eps-greedy.md)
- [SoftMax](https://github.com/kfoofw/bandit_simulations/blob/master/python/analysis/softmax.md)
- [UCB](https://github.com/kfoofw/bandit_simulations/blob/master/python/analysis/ucb.md)
- [Thompson Sampling](https://github.com/kfoofw/bandit_simulations/blob/master/python/analysis/ts.md)

## Special Mention
A portion of the code is based on the book ["Bandit Algorithms for Website Optimization"](https://www.oreilly.com/library/view/bandit-algorithms-for/9781449341565/) by John Myles White.

Microsoft's `vowpal wabbit` package for Python can be found in this [Github repo](https://github.com/VowpalWabbit/vowpal_wabbit).

The R package for `contextual` can be found in this [Github repo](https://github.com/Nth-iteration-labs/contextual).



