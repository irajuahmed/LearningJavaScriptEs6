<h1 align="center">Set Object</h1>

In JavaScript `Set` is a collection of unique values. `Set` can hold any value of any data type & the elements in `sets` are iterated in their insertion order. `Set` is the collection of values similar to arrays, but it does not contain any duplicates.

## Characteristics:
- Value of `Set` must be unique means a value in the `Set` may only occur once. 
- It can hold any data type.
- It shows data as it insertion order.
- `Set` does not have index.
- A `Set` has no keys.

## Set Methods:
<table align="left" width="100%">
<tr>
    <th>Method Name</th>
    <th>Description</th>
    <th>Example</th>
</tr>
<tr>
  <td>new Set()</td>
  <td>Creates a new Set</td>
  <td>
        <pre lang="Javascript">
           const letters = new Set(["a","b","c"]);
           const profession = new Set("bookkeepers");
        </pre>
    </td>
</tr>
<tr>
    <td>add()</td>
    <td>Adds a new element to the Set</td>
    <td>
        <pre lang="Javascript">
           const letters = new Set();           
           letters.add("a");
        </pre>
    </td>
</tr>
<tr>
    <td>delete()</td>
    <td>Removes an element from a Set</td>
    <td>
        <pre lang="Javascript">
            let colors = new Set();  
            colors.add('Violet');  
            colors.add('Indigo');  
            colors.add('Violet');  
            console.log(colors);
            colors.delete('Violet');   
            console.log(colors);
        </pre>
        <pre lang="Javascript"> Result in console
        Set(3) {'Violet', 'Indigo', 'Blue'}
        Set(2) {'Indigo', 'Blue'}
        </pre>        
    </td>
</tr>
<tr>
    <td>has()</td>
    <td>Returns true if a value exists</td>
    <td>
        <pre lang="Javascript">
                let colors = new Set(['Green', 'Red', 'Orange', 'Yellow', 'Red']);  
                colors.add('Violet');  
                colors.add('Indigo');  
                colors.add('Blue');  
                colors.add('Violet');  
                console.log(colors.has('Indigo'));  
                console.log(colors.has('Violet'));  
                console.log(colors.has('Cyan')); 
        </pre>
        <pre lang="Javascript"> Result in console:
        true
        true
        false
        </pre>  
    </td>
</tr>
<tr>
    <td>clear()</td>
    <td>CRemoves all elements from a Set</td>
    <td>
        <pre lang="Javascript">
            let colors = new Set(['Green', 'Red', 'Orange', 'Yellow', 'Red']);  
            colors.add('Violet');  
            colors.add('Indigo');  
            colors.add('Blue');  
            colors.add('Violet');  
            colors.clear();
            console.log(colors.size);
        </pre>
        <pre lang="Javascript"> Result in console:
        
        0
        </pre> 
    </td>
</tr>
  <tr>
      <td>forEach()</td>
      <td>Invokes a callback for each element</td>
      <td>
        <pre lang="Javascript">

        </pre>
     </td>
</tr>
  <tr>
      <td>values()</td>
      <td>Returns an Iterator with all the values in a Set</td>
      <td>
        <pre lang="Javascript">

        </pre>
    </td>
</tr>
  <tr>
      <td>keys()</td>
      <td>Same as values()</td>
      <td>
        <pre lang="Javascript">

        </pre>
    </td>
</tr>
<tr>
    <td>entries()</td>
    <td>Returns an Iterator with the [value,value] pairs from a Set</td>
    <td>
        <pre lang="Javascript">

        </pre>
    </td>
</tr>
