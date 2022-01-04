# Linear-Programming-Iventory_Problem
example 3.6-1 Operations Research An Introduction by Hamdy A. Taha  JOBCO manufactures two products on two machines. A unit of product 1 requires 2 hrs on machine 1 and 1 hr on machine 2. For product 2, one unit requires 1 hr on machine 1 and 3 hrs on machine 2. The revenues per unit of products 1 and 2 are $30 and $20, respectively. The total daily processing time available for each machine is 8 hrs. Letting x1 and x2 represent the daily number of units of products 1 and 2, respectively.


GLPK 5.0  - SENSITIVITY ANALYSIS REPORT                                                                         Page   1

Problem:    
Objective:  _objective = 128 (MAXimum)

   No. Row name     St      Activity         Slack   Lower bound       Activity      Obj coef  Obj value at Limiting
                                          Marginal   Upper bound          range         range   break point variable
------ ------------ -- ------------- ------------- -------------  ------------- ------------- ------------- ------------
     1 machine1     NU       8.00000        .               -Inf        2.66667     -14.00000      53.33333 machine1
                                          14.00000       8.00000       16.00000          +Inf     240.00000 machine_2

     2 machine2     NU       8.00000        .               -Inf        4.00000      -2.00000     120.00000 machine_2
                                           2.00000       8.00000       24.00000          +Inf     160.00000 machine1


Changes in the right hand:
The conclusion is that the dual price of $14.00/hr remains valid only in the range 2.67 hr … Machine 1 capacity … 16 hr -
	The rate of change in optimum z resulting from changing machine 1 capacity in 1 unit can be computed as $14.00/hr
Thus, the dual price of $2/hr for machine 2 remains applicable for the range 4 hr … Machine 2 capacity … 24 hr
	The rate of change in optimum z resulting from changing machine 2 capacity in 1 unit can be computed as $2.00/hr


GLPK 5.0  - SENSITIVITY ANALYSIS REPORT                                                                         Page   2

Problem:    
Objective:  _objective = 128 (MAXimum)

   No. Column name  St      Activity      Obj coef   Lower bound       Activity      Obj coef  Obj value at Limiting
                                          Marginal   Upper bound          range         range   break point variable
------ ------------ -- ------------- ------------- -------------  ------------- ------------- ------------- ------------
     1 machine1     BS       3.20000      30.00000        .                -Inf       6.66667      53.33333 machine1
                                            .               +Inf        4.00000      40.00000     160.00000 machine2

     2 machine_2    BS       1.60000      20.00000        .                -Inf      15.00000     120.00000 machine2
                                            .               +Inf        2.66667      90.00000     240.00000 machine1

End of report

changes in the Objective coefficients
Maximinze z = c1x1 + c2x2

53.33/160<=c1/c2<=240/120
