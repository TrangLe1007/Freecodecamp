function getIndexToIns(arr, num) {
  arr.sort(function(a, b) {
    return a - b;
  });

  for(var i = 0; i< arr.length; i++){
    if(arr[i] >= num){
      return i;
    }
  }
  return arr.length;
  // if don't have the value which is greater than num, the output will be arr.length;
}

console.log(getIndexToIns([40, 60], 50));
