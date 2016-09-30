/* https://www.hackerrank.com/challenges/30-2d-arrays */

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
    var arr = [];
    for(arr_i = 0; arr_i < 6; arr_i++){
       arr[arr_i] = readLine().split(' ');
       arr[arr_i] = arr[arr_i].map(Number);
    }
    
    var sumarr = [];
    
    var h = 0;
    for (var i = 0; i < 4; i++) {
        for (var j = 0; j < 4; j++) {
            sumarr[h] = arr[i][j] + arr[i][j+1] + arr[i][j+2]
                    + arr[i+1][j+1] + arr[i+2][j] + arr[i+2][j+1]
                    + arr[i+2][j+2];
            h++;
        }
    }

    sumarr.sort();
    
    var max = -99999;
    for (var x = 0; x < 16; x++){
        if (sumarr[x] > max)
            max = sumarr[x];
    }
    
    console.log(max);
}

