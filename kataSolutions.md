Sum of differences in array


function sumOfDifferences(arr) {
  let sorted = arr.sort((a, b) => b - a);
  //console.log.(sorted)
  let sum = 0;
    for(let i = 0; i < sorted.length - 1; i++){
      sum = sum + (sorted[i] - sorted[i+1]);
    }
    return sum;
}