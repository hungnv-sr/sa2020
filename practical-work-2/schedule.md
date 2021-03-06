## FCFS
```
	*--------------------*
	|       P1: A:0 B:5  |
	*--------------------*
	|
	|   *------------*
	|   | P2: A:1 B:3|---*
	|   *------------*   |
  	|                    |
   	|                    |   *-------*
   	|                    |   | P3    |:5.5 B:2
   	|                    |   *-------**
	|                    |            |
	|                    |         *---*
	|                    |         |P4 | A:6.8 B:1
	|                    |         *---*-------*
	|                    v            v        v
	*--------------------*------------*--------*----*
	|       P1: B:5      | P2: B:3    |P3 B:2  | P4 |
	*--------------------*------------*--------*----*
```

Average waiting time: (0 + 4 + 2.5 + 3.2 )/4 = 2.425 (ms)

Average turnaround time: (5 + 7 + 4.5 + 4.2) / 4 = 5.175 (ms)


## SJF

```
	*--------------------*
	|       P1: A:0 B:5  |
	*--------------------*
	|
	|   *------------*
	|   | P2: A:1 B:3|---*
	|   *------------*   |
  	|                    |
   	|                    |   *-------*
   	|                    |   | P3    |:5.5 B:2
   	|                    |   *-------*-----*
	|                    |            |    |
	|                    |         *---*   |
	|                    |         |P4 | A:6.8 B:1
	|                    |         *---*   |
	|                    v            v    v
	*--------------------*------------*----*--------*
	|       P1: B:5      | P2: B:3    | P4 | P3     |
	*--------------------*------------*----*--------*
```

Average waiting time: (0 + 4 + 3.5 + 1.2 )/4 = 2.175 (ms)

Average turnaround time: (5 + 7 + 5.5 + 2.2) / 4 = 4.925 (ms)

## SRTF

```
	*--------------------*
	|       P1: A:0 B:5  |
	*--------------------*
	|
	|   *------------*
	|   | P2: A:1 B:3|
	|   *------------*   
  	|   |                 
   	|   |                    *-------*
   	|   |                    | P3    |:5.5 B:2
   	|   |                    *-------*
	|   |                    |        
	|   |                    |     *---*
	|   |                    |     |P4 | A:6.8 B:1
	|   |                    |     *---*
	|   v                    v        v
	*---*------------*---*---*--------*----*--------*
	|P1 |   P2       |P1     | B:3    | P4 | P1     |
	*---*------------*---*---*--------*----*--------*
```

Average waiting time: (6 + 0 + 0 + 0.7 )/4 = 1.675 (ms)

Average turnaround time: (11 + 3 + 2 + 1.7) / 4 = 4.425 (ms)


## RR

```
	*-----------------------*
	|       P1: A:0 B:5     |
	*-----------------------*
	|
	|    *-------------*
	|    | P2: A:1 B:3 |
	|    *-------------*   
  	|    |                 
   	|    |                     *--------*
   	|    |                     | P3     |:5.5 B:2
   	|    |                     *--------*
	|    |                     |        
	|    |                     |     *----*
	|    |                     |     |P4  | A:6.8 B:1
	|    |                     |     *----*
	|    v                     v     v
	*----*----*----*----*----*----*----*----*----*----*----*
	|P1  |P2  |P1  |P2  |P1  |P2  |P3  |P4  |P1  |P3  |P1  |
	*----*----*----*----*----*----*----*----*----*----*----*
```

Average waiting time: (6 + 2 + 2.5 + 0.2 )/4 = 2.675 (ms)

Average turnaround time: (11 + 5 + 4.5 + 1.2) / 4 = 5.425 (ms)
