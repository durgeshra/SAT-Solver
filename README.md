Assignment 2: Implementing a SAT solver using semantic tableaux
Done by: Shivam Kumar (170669) and Durgesh Agrawal(170262)

Executing the Program:
Paste the 'sat_solver.py' file in the same directory having the input file "input.txt".Then open terminal and run 'python sat_solver.py'.

Output of the program:
The program emits output in the file "output.txt" exactly in the same format as that of the minisat i.e. if the formula is satisfiable, it prints "SAT" without the double quotes and then a model solution in the output file , otherwise it just prints "UNSAT".

Understanding the code:
The code uses the method of semantic tableaux to decide the satisfiability of the propositional logic formulae in cnf form.
SELECTING CLAUSE: The program keeps a separate memory of the length of the clauses and selects the clause with smallest length for the decomposition.
SELECTING LITERALS: After selecting a clause, the program assigns a "TRUE" value to that literal which is present in the maximum number of clauses.
OTHER HEURISTICS: After the assignment to the literal, the program uses the method of unit-propagation, DPLL and Boolean Constrain Propagation(BCP) to reduce the number of decompositions involved.
Running time of a normal sudoku given in the assignment 1: 3.329 seconds
