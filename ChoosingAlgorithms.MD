https://machinelearningmastery.com/a-data-driven-approach-to-machine-learning/

If You Knew Which Algorithm or Algorithm Configuration To Use,
You Would Not Need To Use Machine Learning
There is no best machine learning algorithm or algorithm parameters.

I want to cure you of this type of silver bullet mindset.

I see these questions a lot, even daily:

* Which is the best machine learning algorithm?
* What is the mapping between machine learning algorithms and problems?
* What are the best parameters for a machine learning algorithm?
* There is a pattern to these questions.

You generally do not and cannot know the answers to these questions beforehand. You must discover it through empirical study.

There are some broad brush heuristics to answer these questions, but even these can trip you up if you are looking to get the most from an algorithm or a problem.

In this post, I want to encourage you to break free of this mindset and take hold of a data-driven approach that is going to change they way you approach machine learning.

## Best Machine Learning Algorithm
Some algorithms have more “power” than others. They are non-parametric or highly flexible and adaptive, or highly self-tuning or all of the above.

Typically this power comes at a cost of difficulty to implement, the need for very large datasets, limited scalability, or a large number of coefficients that may result in over-fitting.

With bigger datasets, there has been a renewed interest in simpler methods that scale and perform well.

Which is the best algorithm, the algorithm that you should always try and spend the most time learning?

I could throw out some names, but the smartest answer is “none” and “all“.

## No Best Machine Learning Algorithm
You cannot know a priori which algorithm will be best suited for your problem.

Read the above line again. Meditate on it.

Meditate on it.
* You can apply your favorite algorithm.
* You can apply the algorithm recommended in a book or paper.
* You can apply the algorithm that is winning the most Kaggle competitions right now.
* You can apply the algorithm that works best with your test rig, infrastructure, database, or whatever.
These are biases.

They are short-cuts in thinking that save time. Some may, in fact, be very useful short-cuts, but which ones?

By definition, biases will limit the solutions that you can achieve, the accuracy you can achieve, and ultimately the impact that you can have.

## Mapping of Algorithms to Problems
There are general classes of problems, say supervised problems like classification and regression and unsupervised problems like manifold learning and clustering.

There are more specific instances of these problems in sub-fields of machine learning like Computer Vision, Natural Language Processing and Speech Processing. We can also go the other way, more abstract and consider all of these problems as instances of function approximation and function optimization.

* You can map algorithms to classes of problems, for example, there are algorithms that can handle supervised regression problems and supervised classification problems, and both types of problems.
* You can also construct catalogs of algorithms, and that may be useful to inspire you as to which algorithms to try.
* You can race algorithms on a problem and report the results. Sometimes this is called a bake-off and is popular in some conference proceedings for presenting new algorithms.

## Limited Transferability of Algorithm Results
Generally, racing algorithms is anti-intellectual. It is rarely scientifically rigorous (apples to apples).

A key problem with racing algorithms is that you cannot easily transfer the findings from one problem to another. If you believe this statement is true, then reading about algorithm races in papers and blogs does not inform you about which algorithm to try on your problem.

If algorithm A kills algorithm B on Problem X, what does that tell you about algorithm A and B on problem Y? You have to work to relate problems X and Y. Do they have the same or similar properties (attributes, attribute distributions, functional form) that are exploited by the algorithms under study? That’s some hard work.

We do not have fine-grained understandings of when one machine learning algorithm works better than another.

## Best Algorithm Parameters
Machine learning algorithms are parametrized so that you can tailor their behavior and results to your problem.

The problem is that “how” to do the tailoring is rarely (if ever) explained. Often, it is poorly understood, even by the algorithm developers themselves.

Generally, machine learning algorithms with stochastic elements are complex systems and must be studied as such. The first order – what effect does the parameter have on the complex system may be described. If so, you may have available some heuristics on how to configure the algorithm as a system.

It is the second order, what effect will it have on your results which is not known. Sometimes you can talk in generalities about the parameters’ effects on the algorithm as a system and how this translates to classes of problem, often not.

No Best Algorithm Parameters
New sets of algorithm configurations are essentially new instances of algorithms for you to challenge your problem (albeit, relatively constrained or similar in the results they can achieve).

You cannot know the best algorithm parameters for your problem a priori.

* You can use the parameters used in the seminal paper.
* You can use the parameters in a book.
* You can use the parameters listed in a “how I did it” kaggle post.
Good rules of thumb. Right? Maybe, maybe not.

## Data-Driven Approach
We do not need to fall into a heap of despair. We become scientists.

You have biases that can short-cut decisions for algorithm selection and algorithm parameter selection. They can serve you well in many cases, we think.

I want you to challenge this, to consider abandoning heuristics and best practices and take on a data-driven approach to algorithm selection.

Rather than picking your favorite algorithm, try 10 or 20 algorithms.

Double down on those that show signs of being better in performance, robustness, speed or whatever concerns interest you most.

Rather than picking the common parameters, grid search tens, hundreds or thousands of combinations of parameters.

Become the objective scientist, leave behind anecdotes and study the intersection of complex learning systems and data observations from your problem domain.

This is a powerful approach that requires less up-front knowledge, but a lot more back-end computation and experimentation.

As such, you will very likely be required to work with a smaller sample of your dataset so that you can get results quickly. You will want a test harness that you can have complete faith in.

Side note: how can you have complete trust in your test harness?

You develop trust by selecting the test options in a data-driven manner that gives you objective confidence that your chosen configuration is reliable. The type of estimation method (split, boosting, k-fold cross validation, etc.) and it’s configuration (size of k, etc.).

## Fast Robust Results
You get good results, fast.

If random forest is your favorite algorithm, you could spend days or weeks trying in vain to get the most from the algorithm on your problem, which may not be suited to the method in the first place. With a data-driven methodology, you can discount (relative) poor performers early. You can fail fast.

It takes discipline to not fall back on biases and favorite algorithms and configurations. It’s hard work to get good and robust results.

The result is that you no longer care about algorithm hype, it’s just another method to include in your spot checking suite. You no longer fret over whether you’re missing out by not using algorithm X or Y or configuration A or B (fear of loss), you throw them in the mix.

## Leverage Automation
The data-driven approach is a problem of search. You can leverage automation.

You can write re-usable scripts to search the for the most reliable test harness for your problem before you begin. No more ad hoc guessing.

You can write a reusable script to try automatically 10, 20, 100 algorithms across a variety of libraries and implementations. No more favorite algorithms or libraries.

The line between different algorithms is gone. A new parameter configuration is a new algorithm. You can write re-usable scripts to grid or random search each algorithm to truly sample its capability.

Add feature engineering on the front so that each “view” on the data is a new problem for algorithms to be challenged against. Bolt-on ensembles at the end to combine some or all results (meta-algorithms).

I have been down this rabbit hole. It’s a powerful mindset and it gets robust results.

## Summary
In this post, we have looked at the common heuristic and best-practice approach to algorithm and algorithm parameter selection.

We have considered that this approach leads to limitations in our thinking. We yearn for silver bullet general purpose best algorithms and best algorithm configurations, when no such things exist.

There is no best general purpose machine learning algorithm.
There are no best general purpose machine learning algorithm parameters.
The transferability of capability for an algorithm from one problem to another is questionable.
The solution is to become the scientist and to study algorithms on our problems.

We must take a data-driven problem, to spot check algorithms, to grid search algorithm parameters and to quickly find methods that yield good results, reliably and fast.
