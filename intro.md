# the Husky Programming Language

## Introduction

Today, everything is about AI, and AI is about function approximation. The most successful function approximation methods to date are end-to-end deep learning models like transformers, relying on massive compute and data rather than a priori knowledge. However, it's questionable whether this is the only thing we shall need to progress towards AGI. Dispute aside, we are here to provide essential toolings for exploring alternative and complementary paths besides end to end function approximation. The new AI paths are hybrid AI models. These toolings take the form of a new programming language, called Husky.

### Hybrid AI

It's basically the same as compound AI system defined in https://bair.berkeley.edu/blog/2024/02/18/compound-ai-systems/. However, we want to use a different term to avoid later confusion if things evolve towards different directions.

Here, hybrid AI means an AI that combines models trained independently to form an organic entity, as contrary to the end-to-end approach.  Each component can be a neural network, obtained from an end-to-end training procedure, a hard coded function written by human experts, or a symbolic rule system with rules either collected or learned. We must stress that, the word "hybrid" is meant be the opposite of end-to-end, meaning the components are not trained simultaneously connected together. So a hybrid AI system can even be composed purely neural networks.

TODO: explain possible benefits of Hybrid AI.

Now a hybrid AI system should be able to ***automatically train and compose the individual components***. It's harder than it sounds. Each individual component should be given the proper dataset, filtered to a specific purpose, enabling the system to vastly exploit the structure of the task at hand. Moreover, a hybrid AI system could potentially be able to ***adapt its architecture to specific circumstances***.

### Husky Programming Language

The Husky programming language is designed to faciliate development of new Hybrid AI systems. It's not meant to be perfect, but meant to be provocative, stimulate as much innovation as possible. Thus, it has the following design goals:

- **development in one language**. It's a pain to switch languages. Husky is targeted towards Hybrid AI, which shall combines things that we typically use different languages to write, including Python, Lisp, Coq, Ocaml, Haskell, etc. Husky is designed to be able to write all possible genres of AI as smoothly as possible.
- **builtin language constructs for hybrid AI components and high level expressions to create and combine them.** In most existing languages, everything is understood as a value. To elevate above the level of values, one resorts to complicated abstractions and macros and type tricks and sugars (like Monads, lisp macros, etc). In Husky, we fully avoid these things yet able to provide the right abstraction level for the development of hybrid AI. Roughly speaking, in Husky one can easily define a value that depends on one or several global variables, and the dependency is statically known. Then it can be viewed either as just a value or a function of one or several variables, depending on circumstances. As we shall see, this frees up a lot of language design possibilitie which we shall exploit to facilite hybrid AI development. 
- **extremely convenient debugging**. Debugging is notoriously one of the most time consuming part of software development and computer science research. However, rarely debugging is considered at the language design level. The Husky programming language has higher level builtin notions that allows debugger to present the computation progress in a timeless tree form, allowing quickly locating bugs.

## Development in One Language

## Ascension

## Debugger
