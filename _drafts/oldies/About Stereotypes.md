I was surprised a few days ago when suddenly I've asked myself (and my job mate Mike), why in the name of gods I'm separating the unit tests from the code they covers in the special project named `MyProjectTests`? That was a part of my why-game I'm playing last months when trying to improve my coding productivity by paying attention for all these small parts of my daily process I'd like to change easily and in natural way without blowing my mind out. 

Briefly, the most annoyed thing induced me to raise this question was the fact that I'm jumping between two projects and between two source trees when I'm working on the one solid stuff. When I start to code a new feature I mostly write all code in one file in TDD fast track manner without taking care about entire project structure this code will fit with at least on the early stages. That allows me to keep the focus as long as possible within a task boundaries and to find abstract solutions for the complex problems. And I feel sad when I need to split the classes into separated files and projects as it fires me to use different workflow.

I'll not dive deeper into this topic as it's a subject for a separated discussion is already covered in lots of other post you can always find in the web. This case is less important than the bigger picture I saw in all these small questions and I can head them all as:

### How stereotypic our decision are?

How usually engineers makes technical decisions in the complex domains? They work with stereotypic problem specific solutions bundles named 'patters'. The using some intuitive and abstract criterias for finding the appropriated pattern and then **fully trust** them. And it's a great idea to have some experts approved solutions you can just apply to your design.

But this trust plays a bad role in forming a *cult of patterns*, which is based on unfounded application of the patterns when the much better solution would be used.

Let's remember a few of the most significant cases in my opinion that illustrate few different stereotypes evolution curves.

### Singleton

It was a truly epic. From ages ago programmers used to use the global variables in their programs to store some state data and share it between modules. And every new programming language had something like `static` keyword. It was a trade-off for those who lived in world of procedural CPU-oriented programming models and who wanted to bring the usual approaches to the modern paradigms. This pattern was improved few times and formalized in a kind of *canonical* double-locking form. But every grade-school student knows that using the global variables is a way to hell and in same time everybody kept to believe that *singleton* is something... Well, maybe not different, but justifying usage of the hateful global variables.

And what we are observing today? Saying the word 'singleton' on the interview may kill your career! The glorious *pattern* today is known as a worst *anti-pattern* that kills applications performance on the modern multi-CPU platforms.

And today it doesn't look unnatural to not use it at all even in old-fashioned programs. It just gone in same way like *goto* operator, but few decades ago all programs was a mix of 'jumps' from line to line.

### Object-Oriented Programming

What is the foundation of the object-oriented design? From the university courses we should remember these three words: **encapsulation**, **inheritance** and **polymorphism**. These concept describes all power of the object-orientation when you can reuse complex abstract program components in extremely flexible way. On your C++ programs you can use 'public' and 'private' variables within a 'class', substitute functions implementations with virtual calls table and inherit a single class from a whole world. This is a god's power!

And then one day was released a new language named JAVA where multi-inheritance was killed. Oh, how people cried about this *pattern*! 

But what we have today? Yes, the industrial languages still support most of 'old' keywords, but we can see how SOLID-movement exposing the old practices: *inheritance* should be replaced with *composition*, the *polymorphic* hierarchies should be replaced with *interfaces implementations*, and even the private fields within the classes are just a kind of class scope *singletons*. 

### Relational Data Modeling



### Transactional Business Operations




