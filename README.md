# Automatic Parallelisation using Effect Tracking and Cost Analysis 

**Award-winning**. Awarded the CST Department Prize for a Highly Commended Dissertation in the Computer Science Tripos for Part II 2023. 

An _automatic-parallelisation_ compiler written in OCaml: compiling a user-annotated subset of sequential Go code into multithreaded Go code. 

Utilises a mixture of _effect tracking_ and _cost analysis_. Effect tracking determines whether two blocks of code can be run concurrently without interfering. Cost analysis combines _static_ and _dynamic_ analysis, to estimate both data-structure sizes and execution times for programs. This allows us to estimate whether parallelising two blocks of code will provide a runtime improvement. If blocks of code can be parallelised to reduce the program's runtime without interfering with each other, they are compiled into their parallelised form in the resulting multithreaded Go code.
