# codegolf

My experiments with codegolfing

Language Javascript , ES6
    1. Days of a month in a non-leap year
       m=(n)=>(15662007>>(n-1)*2&3)|28
       
    2. Repeating a string n number of times in O(log n) complexity
       f=(s,n)=>n?['',s][n&1] + f(s+s,n>>1):''
    
    3. Base 64 encoding (under progress)
       b64=n=>{var hash = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/';             return[...n].map(x=>'00000000'.slice(Math.ceil(Math.log2(x.charCodeAt(0)))) + x.charCodeAt(0).toString(2)).join('').match(/.{6}/g).map(x=>hash[parseInt(x,2)])}
