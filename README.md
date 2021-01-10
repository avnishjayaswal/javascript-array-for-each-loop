javascript forEach()  method calls a function once for each element in an array , callback function is not executed for array elements without values.

for each code example

we have a array like

```javascript
const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9];
```

The forEach (<a href="https://askavy.com/javascript-each/">javascript each</a>) method use a callback function for each element of an array with 3 parameters

1 – array item
2 – array index
3 – array

array item (value) parameter in for each loop

```javascript

     const numbers = [1, 2, 3, 4, ];
     numbers.forEach((item) => {
       document.write(item) ;      // output 1 2 3 4
       document.write("<br />") ;
     }) ;
```

optional parameter index in foreach method

```javascript

      const numbers = [1, 2, 3, 4];
      numbers.forEach((item, index) => {
        console.log("Index: " + index + " Value: " + item);
      });

Output
Index: 0 Value: 1
Index: 1 Value: 2
Index: 2 Value: 3
Index: 3 Value: 4

```

array parameter in foreach method

```javascript

      const numb

ers = [1, 2, 3, 4];
      numbers.forEach((item, index , array) => {
        console.log("Index: " + index + " Value: " + item + " array " + array);
      });
OutPut 
Index: 0 Value: 1 array 1,2,3,4
Index: 1 Value: 2 array 1,2,3,4
Index: 2 Value: 3 array 1,2,3,4
Index: 3 Value: 4 array 1,2,3,4

```

javascript array foreach using key and value


```javascript

      const numbers = [1, 2, 3, 4];
      numbers.forEach((value, key) => {
        console.log("key: " + key + " Value: " + value );
      });

```

javascript foreach object

```javascript
     const obj = {
        name: "value1",
        rank: "value2",
      };

     Object.keys(obj).forEach((key) => {
        console.log(key, obj[key]);
      });

Output
name value1
rank value2
```

The Object.values() function return an array with index and values

```javascript

    const obj = {
        name: "Avy",
        rank: "Captain",
      };

      Object.values(obj).forEach((val) => {
        console.log(val);
      });

OutPut
Avy
Captain

```

The Object.entries() function returns an array of entries. An entry is an array of length 2, where entry[0] is the key and entry[1] is the value

```javascript

      const obj = {
        name: "Avy",
        rank: "Captain",
      };

      Object.entries(obj).forEach((entry) => {
        const [key, value] = entry;
        console.log(key, value);
      });

OutPut
name Avy
rank Captain


```






