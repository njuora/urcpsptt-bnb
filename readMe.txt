This is the results of the research article: A Branch-and-Bound Algorithm for the Unit-Capacity Resource Constrained Project Scheduling Problem with Transfer Times (Ying Liu, Shuang Jin, Jing Zhou, Qian Hu)

1. urcpsptt-bnb.xlsx: the results of the BNB algorithm for the urcpsptt

- BNB: the results of the BNB
- BNB-DR: test for different dominance rules
- BNB-LB: test for different lower bounds
- BNB(+GRASP): the results of using the GRASP to generate an initial upper bound before BNB

2. urcpsptt-cp.xlsx: the results of CP for the urcpsptt

- cp: results of CP
- cp with grasp: the results of using the GRASP to generate an initial upper bound before CP

3. urcpsptt-cplex.xlsx: the results of CPLEX for the urcpsptt

- cplex: results of CPLEX
- cplex with grasp: the results of using the GRASP to generate an initial upper bound before CPLEX

4. rcpsp-bnb.xlsx: the results of the BNB algorithm for the RCPSP

- BNB: results of the BNB
- BNB-DR: test for different dominance rules
- Best known solution: the best known solutions in the literature (till 20220822)

5. urcpsptt-tables.xlsx: summary tables for the urcpsptt and rcpsp

*****
 urcpsptt-sol, rcpsp-sol: detailed solutions for all benckmark instances

 rcpsp: 2040 instances in the PSPLIB library
 urcpsptt: 432 instances from  (Liu et al., 2021): https://github.com/njuora/urcpsptt

 note that in every solution, the activities are renumbered according to a tologolical ordering (contained in the sol folder)

