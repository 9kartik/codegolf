# codegolf

My experiments with codegolfing

Language Javascript , ES6
    1. Days of a month in a non-leap year
       m=(n)=>(15662007>>(n-1)*2&3)|28
       
    2. Repeating a string n number of times in O(log n) complexity
       f=(s,n)=>n?['',s][n&1] + f(s+s,n>>1):''
