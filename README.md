Download Link : https://programming.engineering/product/ve477-homework-2/

# VE477-Homework-2
VE477 Homework 2

Questions preceded by a * are optional. Although they can be skipped without any deduction, it is important to know and understand the results they contain.

Ex. 1 — Basic complexity

1. Prove that

a) n3 − 3n2 − n + 1 = Θ(n3); * c) ∀a ∈ R, b ∈ R+, (n + a)b = Θ(nb );

        n2 = O(2n);

    For each pair of functions state whether f (n) = O(g (n), f (n)Ω(g (n)), f (n) = Θ(g (n)), or none.

    	

    a) f (n) = n√
    			

    , g (n) = n2 − 1;
    	

    * b) f (n) = 2n − n2, g (n) = n4 + n2;
    	

    n

    3.
    	

    Find two functions f (n) and g (n) such that
    					
    	

    a) f (n) = Θ(g (n)) and f (n) ̸= O(g (n))
    	

    b) f (n) = Ω(g (n)) and f (n) ̸= O(g (n))

    4.
    	

    Order the following functions into increasing asymptotic order.
    				
    	

    a) f (n) =
    		

    n
    	

    √
    							
    	

    i
    	

    c) f3(n) = n
    	

    log n
    	

    1
    		

    i =1
    	
    	

    f (n) = √n log n
    	

    n
    	

    2 + 4n + 6
    										

    d) f4(n) = 24√
    	

    3
    	
    	

    b) 2
    	

    ∑
    			
    							

Ex. 2 — Master Theorem

The goal of this exercise is to prove the Master Theorem (2.??) in the case where n is a power of b > 1. Both n and b, as well as all the other notations are similar to the ones used in the lecture slides. The only slight difference is that n is to be explicitly taken as an exact power of b.

    We want to transform the evaluation of the master recurrence into a summation.

        Draw the recursion tree corresponding to the master recurrence.

        Determine

i – The depth of the tree;

            – The number of leaves;

            – The total cost for the all the nodes at each depth;

            – Conclude that

                            	

                            logb n−1
                            	

                            T (n) = Θ(nlogb a) +
                            	

                            ∑j
                            	

                            (2.1)

                            aj f (n/bj ).
                            	

                            =0
                            	

2. To obtain an asymptotic bound on sum (2.1), we focus on its right part and denote it

    		

    logb n−1
    						
    	

    g (n) =
    	

    ∑j
    	

    aj f (n/bj ).
    	
    			
    		

    =0
    							

    a) Assume f (n) = Θ(nlogb a)
    									

    i –
    	

    Prove that
    		

    logb n−1
    					
    					

    n
    	

    logb a
    			

    ∑
    					
    	

    g (n) = Θ
    	

    j =0
    	

    aj
    	

    (bj )
    	

    .

    * ii –
    	

    Show that
    	

    aj (
    		

    )
    						
    	

    logb n−1
    	

    n
    	

    logb a
    				
    	

    ∑
    			

    = nlogb a logb n.
    	

    bj
    	

            =0

        – Conclude that g (n) = Θ(nlogb a log n).

    Assume f (n) = O(nlogb a−ε), ε > 0.

        * i –
        	

        Prove that
        			

        logb n−1
        								
        							

        n
        		

        logb a−ε
        				

        ∑
        								
        	

        g (n) =
        	

        O
        	

        j =0
        	

        aj
        	

        (bj )
        		

        .

        ii –
        	

        Show that
        												
        	

        logb n−1
        		

        n
        	

        logb a−ε
        			

        nε
        		

        1
        	
        	

        ∑ aj
        	

        (
        		

        )
        			

        =
        		

        −
        	

        nlogb a−ε.
        	

        bj
        			

        bε
        	

        − 1

                        =0

                    – Conclude that g (n) = O(nlogb a).

        Assume af (n/b) ≤ cf (n), for some c < 1 and n large enough, and f (n) = Ω(nlogb a+ε), with

                > 0.

i – Observe that g (n) = Ω(f (n)).

                    – Prove that after j iterations aj f (n/bj ) ≤ cj f (n). * iii – Show that g (n) = O(f (n)).

                    – Conclude that g (n) = Θ(f (n)).

    Using the results from questions 1 and 2, derive the Master Theorem as phrased in the lecture slides, in the case where n is an exact power of b.

Ex. 3 — Ramanujam numbers

A Ramanujam number is a positive integer n which can be written from two different ways as the sum of two cubes, i.e. there exists four positive integers a, b, c, and d less than n, such that n = a3 + b3 = c3 + d 3. Given n write some pseudocode to determine all the Ramanujam numbers smaller or equal to n. What is the complexity of the algorithm?

Ex. 4 — Critical thinking

Six pirates, ordered with respect to their seniority, want to share 300 pieces of gold among themselves.

They decide to proceed as follows:

1. The senior-most pirate proposes a way to distribute the coins;

    All the pirates vote;

    If at least half of them agree, the division remains;

    Otherwise he is thrown overboard and the process is repeated with the senior-most remaining pirate;

Assuming all the pirates have proper thinking abilities and desire first to remain alive and second to become rich, how many pirates can remain alive and in that case how is the distribution handled?
