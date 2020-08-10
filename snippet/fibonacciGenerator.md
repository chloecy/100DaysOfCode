<b>Fibonacci sequence</b> is a list of numbers where every number is the sum of the two previous ones.

Create a `fibonacciGenerator(n)`

```
function fibonacciGenerator(n) {
  let output = [];
  if (n === 1) {
    output = [0];
  } else if (n === 2) {
    output = [0, 1];
  } else {
    output = [0, 1];
    for (let i = 2; i < n; i++) {
      output.push(output[output.length - 2] + output[output.length -1]);
    }
  }

  return output;  
}

```
