# A Branch-and-Bound Algorithm for the Unit-Capacity Resource Constrained Project Scheduling Problem with Transfer Times

This repository is maintained by Ying Liu (liuyingsme@smail.nju.edu.cn) and Qian Hu (huqian@nju.edu.cn) to supplement the article '"A Branch-and-Bound Algorithm for the Unit-Capacity Resource Constrained Project Scheduling Problem with Transfer Times" published at *Computers & Operations Research*. It contains

1. `urcpsptt-bnb.xlsx`: the results of the BNB algorithm for the  urcpsptt

   - BNB: the results of the BNB

   - BNB-DR: test for different dominance rules

   - BNB-LB: test for different lower bounds

   - BNB(+GRASP): the results of using the GRASP to generate an initial upper bound before BNB (for response)


2. `urcpsptt-cp.xlsx`: the results of CP for the urcpsptt

   - cp: results of CP

   - cp with grasp: the results of using the GRASP to generate an initial upper bound before CP


3. `urcpsptt-cplex.xlsx`: the results of CPLEX for the urcpsptt

   - cplex: results of CPLEX

   - cplex with grasp: the results of using the GRASP to generate an initial upper bound before CPLEX


4. `rcpsp-bnb.xlsx`: the results of the BNB algorithm for the RCPSP

   - BNB: results of the BNB

   - BNB-DR: test for different dominance rules

   - Best known solution: the best known solutions in the literature (till 20220822)


5. `urcpsptt-tables.xlsx`: summary tables for the urcpsptt and rcpsp

6.  `urcpsptt-sol.zip`, `rcpsp-sol.zip`: detailed solutions for all benchmark instances

   - rcpsp: 2040 instances in the PSPLIB library

   - urcpsptt: 432 instances from  (Liu et al., 2021): https://github.com/njuora/urcpsptt

     It should be noted that in every solution, the activities are renumbered according to a topological ordering (contained in the sol folder)

## Abstract

We study a project scheduling problem where unit-capacity resources and transfer times are involved, and propose a branch-and-bound algorithm to solve it. In the problem, each resource is unique and the time on transferring resources between activities is nonnegligible. The aim is to find a feasible solution consisting of a vector of activity start times and a resource transfer plan so that the project makespan is minimized. Our branch-and-bound algorithm uses a branching scheme to branch over all eligible activities to be scheduled at each node, and a scheduling method to decide the start time of next activity, which must be feasible and no earlier than the start time of the last scheduled activity. Based on the combination of the branching scheme and the scheduling method, five effective dominance rules are designed to speed up the exploration of the branch-and-bound tree. With the dominance rules, multiple identical solutions at different nodes are avoided and a large number of unpromising nodes are pruned. At each node, two lower bounds are computed, and an upper bound is produced by a heuristic using a series of priority rules. Extensive computational experiments are conducted on the benchmark instances of the problem. The results show that our exact algorithm performs significantly better than solving the existing mathematical models for the problem using either CPLEX or CP Optimizer.

## Algorithm

Please email the authors

## Instances

- rcpsp: 2040 instances in the PSPLIB library
- urcpsptt: 432 instances from  (Liu et al., 2021): https://github.com/njuora/urcpsptt

## Results

Extensive computational experiments are conducted to evaluate the performance of the branch-and-bound algorithm. Our algorithms are implemented in Java 460 and single-threaded. The experiments are conducted on a workstation with an Intel Xeon Gold 5220 CPU clocked at 2.20 GHz and 128 GB RAM. All benchmark instances and results are available for downloading.



