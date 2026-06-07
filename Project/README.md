# Minimax Regret Bounds in Stochastic and Adversarial Multi-Armed Bandits

### HDP Project Report

## Overview

This repository contains the study and algorithmic extensions for the $K$-armed multi-armed bandit (MAB) problem under both stochastic and adversarial reward models. The project reviews the interaction protocol, explores why minimax lower bounds scale as $\Omega(\sqrt{nK})$, and surveys representative algorithms capable of achieving $\Theta(\sqrt{nK})$ worst-case regret.

A major focus of this project is addressing the estimator variance inherent in the EXP3 algorithm by introducing mathematically rigorous variance-reduction techniques.

## Key Algorithms Explored

The project analyzes the exploration-exploitation tradeoff and theoretical regret bounds of several foundational algorithms:

* 
**Stochastic Settings:** * **UCB1:** Provides strong instance-dependent bounds based on optimism in the face of uncertainty.


* 
**MOSS:** Modifies the exploration bonus to achieve minimax-optimal $\sqrt{nK}$ worst-case regret.




* 
**Adversarial Settings:** * **EXP3:** An exponential-weight algorithm providing robust adversarial guarantees.


* 
**INF (Implicitly Normalized Forecaster):** Achieves minimax-optimal rates by removing the $\sqrt{\log K}$ factor via implicit normalization.





## Project Extensions: Variance-Reduction for EXP3

Motivated by the potential for high variance in the standard EXP3 inverse propensity estimator $\hat{g}_{i,t} = \frac{g_{I_t,t} \mathbf{1}\{I_t=i\}}{p_{i,t}}$ when $p_{i,t}$ is small , this project introduces two core extensions to improve algorithmic stability.

The theoretical foundation of this project is built upon classical bandit literature, including Robbins (1952), Auer et al. (2002, 2003), Audibert & Bubeck (2009), and Bubeck & Cesa-Bianchi (2012).
