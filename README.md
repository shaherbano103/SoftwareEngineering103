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


Second Summary 
Behind the Intents: An In-depth Empirical Study on Software
Refactoring in Modern Code Review

Modern code review platforms such as Gerrit  is increasingly being adopted in both industrial  and open-source projects. Along code reviews, developers inspect and discuss the quality of each other’s code changes before accepting them. Code refactoring plays a key role in modern code review . Refactorings are rarely ignored during code review . In addition, modern code review increases the awareness of developers on the importance of code refactoring. Refactoring consists of applying one or more structural code transformations (i.e., refactoring operations)  as a means to achieve various developers’ intents  and goals. The intents may vary from pure structural improvement to facilitating feature additions or bug fixes


This paper aimed at better understanding the context and motivations in which developers perform refactorings in modern code review. First, we have employed code review data of two large open source communities. Second, we automatically identified occasions in which developers employed 13 refactoring types during code review. Third, we followed this automated procedure with a manual analysis of all code reviews that employed refactoring operations. The manual analysis consisted of identifying the developers’ intents behind each change, such as new feature, bug fixing, and refactoring. Fourth, we identified the most common refactoring sequences employed during code review and analyzed how developers compose these sequences under different intents. Finally, we investigated how refactoring operations evolve during code review. We observed that refactoring operations are most often used in code reviews that implement new features, accounting for 63% of the code changes we studied. Only in 31% of the code reviews that employed refactoring operations the developers had the explicit intent of refactoring. Such observations indicate that developers more often mix refactoring operations with other changes instead of submitting a code review that only performs refactoring. We also observed that developers compose sequences with more than one refactoring type to support feature additions. Moreover, we observed that developers often compose specific refactoring sequences to support multiple intents. Finally, we noticed that about 75% of refactoring operations remain unchanged during the review process for all studied systems. We observed a similar result when grouping reviews by different intents. However, feature-related changes tend to present the highest rate of refactoring evolution while refactoring-related changes presented the lowest rate. The aforementioned findings serve as recommendations for encouraging the research community and tool builders to come up  with a new generation of refactoring tools that best fit the developers’ intents during refactoring application. Through our results, we shed light that (Section 6): (i) existing approaches should better support the application of different refactoring types when developers apply code changes with mixed intents; and (ii) existing refactoring tools should be more interactive to support developers on composing and evolving refactoring sequences in a step-wise manner.Finally, qualitative studies should be performed in the future to  explain other influential factors governing the decision-making process in refactoring-aware code review




Third Summary 
Artificial Intelligence is becoming increasingly popular with organizations due to the success of Machine Learning and Deep Learning techniques. Using these techniques, data scientists learn from vast amounts of data to enhance behaviour in software-intensive systems. Despite the attractiveness of these techniques, however, there is a lack of systematic and structured design process for developing ML/DL models. The study uses a multiple-case study approach to explore the different activities and challenges data scientists face when developing ML/DL models in software-intensive embedded systems. In addition, we have identified seven different phases in the proposed design process leading to effective model development based on the case study. Iterations identified between phases and events which trigger these iterations optimize the design process for ML/DL models. Lessons learned from this study allow data scientists and engineers to develop high-performance ML/DL models and also bridge the gap between high demand and low supply of data scientists
