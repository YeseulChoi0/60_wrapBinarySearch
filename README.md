# 60_wrapBinarySearch

y = log (base 2) x means the number x that 2 to the y power equals to. 

The graph is curved concave down and has a vertical asymptote at x = 0 (continuously approaching negative infinity) while as x approaches infinity, the graph slowly appraoches infinity.

0. The problem - Find an element x from a list of ordered elements (that may or may not contain x) and return its index (or -1 if it is not in the list). 
1. State the recursive abstraction - When I am asked to find an element x from a list of ordered elements with size n that may or may not contain x, the recursive abstraction can find the element x from a list of ordered elements with size n/2. 
2. Identify the parts of this solution that correspond to the six parts of a generalized recursive solution.

    Solution to solving the base cases:
    
    if( low > hi)  // detect base case
    
    return -2;   // solution to base case
    
  if( comparison == 0)    // detect base case
  
    return pageToCheck; // solution other base case
  
  Solution to the recursive case:
  
    int pageToCheck = (low + hi) / 2;
    
    else
    
        if( comparison < 0)
        
            // findMe's spot precedes pageToCheck
            
            return indexOf_recursive( findMe
            
                                     , low
                                     
                                     , pageToCheck -1); // RECURSIVE ABSTRACTION 
                                     
        else
        
            // findMe's spot follows pageToCheck
            
            return indexOf_recursive( findMe
            
                                    , pageToCheck +1 // RECURSIVE ABSTRACTION 
                                    
                                    , hi);
                                    
    //COMBINER is not applicable in this situation along with the leftover processing because only the part of the list that contains the element is needed for each subsequent step. 
            
