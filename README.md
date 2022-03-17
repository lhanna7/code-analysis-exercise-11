# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

```js
function (actualAge){
  if (actualAge == 1){
    return {
      humanYears: actualAge,
      catYears: 15,
      dogYears: 15,
    }
  }

  if (actualAge == 2){
    return {
      humanYears: actualAge,
      catYears: 24,
      dogYears: 24,
    }
  }

  return {
    humanYears: actualAge,
    catYears: (actualAge - 2) * 4 + 24,
    dogYears: (actualAge - 2) * 5 + 24,
  }
}
```

| Input | Output |
| ----- | ------ |
|  1     |   HY:1 / CY:15 / DY:15     | 
|  20    |  HY:20 / CY:96  / DY:114   | 
|  90    |  HY:90 / CY:376  / DY:464  | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>This program takes the input, actualAge, and provides the output of humanYears, catYears, and dogYears. The first return will only happen if actualAge===1, then will give cat/dogYears the output of 15 and the humanYears output will be 1. The second return will only happen if actualAge===2, then will give cat/dogYears the output of 24 and the humanYears output will be 2. Any number other than 1 or 2 will have to be run through the third return.  </td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
