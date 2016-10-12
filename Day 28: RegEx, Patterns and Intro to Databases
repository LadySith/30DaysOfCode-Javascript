/* https://www.hackerrank.com/challenges/30-regex-patterns */

function main (){
    var n = parseInt(readLine());
    var arr = [];
    for (var i = 0; i < n; i++)
        arr.push(readLine());
    
    var gmail = arr.filter(function(x) { return(x.includes("@gmail.com")) });
    gmail.sort();
    var names = gmail.map(function(x) { return(x.slice(0,x.indexOf(' '))) });
    
    names.forEach(function(name) {
        console.log(name);
    })

}
