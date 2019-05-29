# Ejercicios de ordenamiento

## Ejercicio 1 Insertion Sort
```
function insertionSort(array) {

  for(var i = 1; i < array.length; i++) {
    var temp = array[i];
    for(var j = i - 1; j >= 0 && array[j] > temp; j--) {
      array[j+1] = array[j];
    }
    array[j+1] = temp;
  }

  return array;
}
```

## Ejercicio 2 Selection Sort
```
var selectionSort = function(array) {
    var temp;

    for(var i=0; i<array.length; i++){
        var mi = i;

        for(var j = i + 1; j<array.length; j++) {
            if(array[j] < array[mi])
                mi = j;
        }

        temp = array[i];
        array[i] = array[mi];
        array[mi] = temp;
    }
    return array
};
```
### Ejercicio 3 Bubble Sort
```
function bubble(arr){
 for(let i=0;i<arr.length-1;i++){
  for(let j=i+1;j<arr.length;j++){
    if(arr[i]>arr[j]){
    let aux=arr[i]
    arr[i]=arr[j]
    arr[j]=aux
    }
  }
 }
return arr
}
 ```
