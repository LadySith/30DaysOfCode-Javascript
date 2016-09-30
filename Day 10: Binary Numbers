/* https://www.hackerrank.com/challenges/30-binary-numbers */

process.stdin.resume();
process.stdin.setEncoding('ascii');

var input_stdin = "";
var input_stdin_array = "";
var input_currentline = 0;

process.stdin.on('data', function (data) {
    input_stdin += data;
});

process.stdin.on('end', function () {
    input_stdin_array = input_stdin.split("\n");
    main();    
});

function readLine() {
    return input_stdin_array[input_currentline++];
}

/////////////// ignore above this line ////////////////////

function main() {
    var n = parseInt(readLine());
    var arr = [];
    
    while(n != 0){
        if (n%2 == 0)
            arr.push(0);
        if (n%2 == 1)
            arr.push(1);
        n = Math.floor(n/2);
    }
    
    var max = 0;
    var cur = 0;

    
    for (var i = 0, len = arr.length; i < len; i++) {
        if (arr[i] == 1)
            cur++;
        else if (arr[i] == 0){
            if (cur > max)
                max = cur;
            cur = 0;
        }
    }
    
    if (cur > max)
        max = cur;
    
    console.log(max);
}
