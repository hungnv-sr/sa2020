## FCFS
```
	*--------------------*
	|	    P1: A:0 B:5	 |
	*--------------------*
	|
	|   *------------*
	|   | P2: A:1 B:3|---*
	|   *------------*   |
  	|					 |
   	|					 |   *-------*
   	|					 |   | P3    |:5.5 B:2
   	|					 |   *-------**
	|		             |            |
	|					 |         *---*
	|					 |         |P4 | A:6.8 B:1
	|					 |         *---*-------*
	|                    v            v        v
	*--------------------*------------*--------*----*
	| 		P1: B:5      | P2: B:3    |P3 B:2  | P4 |
	*--------------------*------------*--------*----*
```

Average waiting time: (0 + 4 + 2.5 + 3.2 )/4 = 2.425

Average turnaround time: (5 + 7 + 4.5 + 4.2) / 4 = 5.175