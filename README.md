# SoftwareEngineering103
This Repository is about my Subject Software Engineering Assignment given by Dr Ghulsher Laghari 


Summary of Research Paper 

An Empirical Study of Method Chaining in Java
While some promote method chaining as a good practice for improving code readability, others refer to it as a bad practice that worsens code quality. In this paper, we first investigate whether method chaining is a programming style accepted by real-world programmers. To answer this question, we collected Java repositories on GitHub and analyzed historical trends in the frequency of method chaining. The results of our analysis revealed the increasing use of method chaining; 23.1% of method invocations were part of method chains in 2018, where as only 16.0% were such invocations in 2010. We then explore language features that are helpful to the method-chaining style but have not been supported yet in Java. For this aim, we conducted manual inspections of method chains that are randomly sampled from the collected repositories. We also estimated how effective they are to encourage the method-chaining style if they are adopted in Java.`

Introduction: 
Method chaining is promoted as a good practice that improves the readability of source code. By method chaining, redundant temporary variables and code repetitions are eliminated [8]; related method invocations are grouped into a single expression an expression becomes easy to read from left to right as natural-language texts 

However, at the same time, method chaining is often referred to as a bad practice. In the thread on Stack Overflow  many posts claim that method chaining worsens the readability. For instance, a post says:

If you do everything in a single statement then that is compact, but it is less readable (harder to follow) most of the times than doing it in multiple statements.

Definition of Method Chain
We define a method chain as a sequence of one or more method invocations joined by the “.” symbol. We define the length of a
method chain as the number of invocations in the sequence. For example, the Java code snippet shown in  contains five chains of length 1, one chain of length 2, and one chain of length 3. We used Java Parser to parse a Java file and mined the parsing result for method chains.

We first enumerated the chains of length 1 (not-chained method invocations) from our dataset to obtain the baseline values. If the number of not-chained invocations increases at the same pace as the number of method chains longer than one, we cannot argue that the use of method chaining is growing. Note that, for convenience, we below regard a not-chained invocation as a method chain.

HOW CAN WE EXTEND JAVA?

To investigate what language features (or library design) needs to be supported to encourage the use of the method-chaining style, we manually analyzed randomly-sampled 385 chains and the code around them. Since we are interested in why method invocations are not chained, the population of the random sampling was the chains of all lengths (including non-chained invocations) in 2018.	

We attempted to find code patterns that could be transformed into the method-chaining style if Java supported an appropriate language feature or the library supported appropriate API design. In what follows, we present the found patterns with their description by example and the number of their occurrences in the randomly-sampled dataset. We then present appropriate language features or API design for those patterns. At the end of this subsection, we summarize the estimated ratios of those patterns in the population

CONCLUSION
This paper presented our empirical study of method chaining in Java. Our analysis quantitatively revealed the widespread and in-creasing trend of method chaining. To provide information for future language/library development, we estimated how effective it would be to introduce language features and API design for method chaining.

Although our results support the acceptance of method chaining in the real world, user studies need to be carried out to assert the acceptance. It is also interesting and beneficial for a better understanding of method chaining to investigate why real-world programmers prefer (or do not prefer) method chaining. The issues mentioned in the StackOverflow thread  would be helpful to start such an investigation. All of those studies are our primary future work
