<!-- https://unicode-table.com/en/sets/ -->
<!--https://www.javascripttutorial.net/es6/ -->
<h1 align="center">Set Object</h1>

In JavaScript `Set` is a collection of unique values. `Set` can hold any value of any data type & the elements in `sets` are iterated in their insertion order. `Set` is the collection of values similar to arrays, but it does not contain any duplicates.

## ☞ Characteristics:
- Value of `Set` must be unique means a value in the `Set` may only occur once. 
- It can hold any data type.
- It shows data as it insertion order.
- `Set` does not have index.
- A `Set` has no keys.

## ☞ Set Object Property:
<table align="left" width="100%">
<tr>
    <th>Property Name</th>
    <th>Description</th>
    <th>Example</th>
</tr>
    <tr>
  <td>size</td>
  <td>Returns the number elements in a Set(after removing duplicates)</td>
  <td>
       <pre lang="Javascript">
           let colors = new Set(['Green', 'Red', 'Orange', 'Yellow', 'Red']);  
            colors.add('Violet');   
            console.log(colors.size);
        </pre>
        <pre > Output in console
         &#8594; Set size: 5
        </pre> 
    </td>
</tr>
</table>


## ☞ Set Object Methods:
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
        <pre> Output in console
        &#8594; Set(3) {'Violet', 'Indigo', 'Blue'}
        &#8594; Set(2) {'Indigo', 'Blue'}
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
        <pre> Output in console:
        &#8594; true
        &#8594; true
        &#8594; false
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
        <pre> Output in console:        
        &#8594; &nbsp;
        &#8594; 0
        </pre> 
    </td>
</tr>
  <tr>
      <td>forEach()</td>
      <td>Invokes a callback for each element</td>
      <td>
        <pre lang="Javascript">
            const letters = new Set("Raju");
            let text = "";
            letters.forEach (function(value) {
              text += value + "<br>";
            })
            console.log(text);
        </pre>
        <pre> Output in console:        
        &#8594; R
        &#8594; a
        &#8594; j
        &#8594; u
        </pre> 
     </td>
</tr>
  <tr>
      <td>values()</td>
      <td>Returns an Iterator with all the values in a Set. It returns a new iterator object that includes the values for each element in the Set object in the insertion order.</td>
      <td>
        <pre lang="Javascript">
            let colors = new Set(['Green', 'Red', 'Orange', 'Yellow', 'Red']);  
            var val = colors.values();  
            console.log(val.next().value);   
            console.log(val.next().value);   
            console.log(val.next().value);   
            console.log(val.next().value);   
        </pre>
        <pre> Output in console:
        &#8594; Green
        &#8594; Red
        &#8594; Orange
        &#8594; Yellow
        </pre> 
    </td>
</tr>
  <tr>
      <td>keys()</td>
      <td> A Set has no keys. keys() method returns the same as values().</td>
      <td>
        <pre lang="Javascript">
            let colors = new Set(['Green', 'Red', 'Orange', 'Yellow', 'Red']);  
            var itr = colors.keys();   
            console.log(itr.next());   
            console.log(itr.next().value);    
        </pre>
        <pre> Output in console:
          &#8594; {value: 'Green', done: false}
          &#8594; Red
        </pre> 
    </td>
</tr>
<tr>
    <td>entries()</td>
    <td>Returns an Iterator with [value,value] pairs instead of [key,value] pairs.</td>
    <td>
        <pre lang="Javascript">
                let colors = new Set(['Green', 'Red', 'Orange']);  
                colors.add('Violet');   
                var iterator = colors.entries();  
                for (const entry of iterator) {
                console.log(entry); 
                }
        </pre>
        <pre> Output in console:
          &#8594; (2) ['Green', 'Green']
          &#8594; (2) ['Red', 'Red']
          &#8594; (2) ['Orange', 'Orange']
          &#8594; (2) ['Violet', 'Violet']
        </pre> 
    </td>
</tr>
