Javascipt in HTML:

```html
<script src="file.js"></script>
(this is in the same folder)
```

Strict Mode:

    'use strict';   //Put at top of document, helps us and blocks us from stuff and gives us error info

Snippets:

    Use global snippets in VSCode to make work faster

Alert Box:

    alert('message');
    prompt(``);              //Can store in variable
        variable = prompt();

Value:

    Primitive:
        const name = variable;          //cant change leave it what it is
        var name = variable;
        let name = variable;
            let name;                   //dont have define types
            7 types:
                Number: = #
                String: = ''
                Boolean: = true/false
                Undefined: let name;    //can define more than one at a time
                Null: = Null
                Symbol: value that cant change
                BigInt: Large Ints
        let name = "";
            Number(name);               //Change types

Literals:

    String:
        "Text and" + variable
            \n\ -   skip line
    Template:
        `Text and ${variable}`  //above tab
            ENTER - skip line

Operators:

    Math Operators:
        -   //Minus
        +   //plus
        /   //div
        *   //times
        **  //power
    Assignment Operators:
        ++,--           //interate
        +=,-=,*=,/=     //interate by more/less
    Comparison operators:
        >,<, >=, <=
    Equality operators:
        ===             //No Type Conversion
        ==              //Type Coercion
    Nonequal Operator:
        !==             //No Conversion
        !=              //Coercion
    Boolean Operator:
    &&                  //AND
    ||                  //OR
    !                   //NOT

Conditionals:

    if() result;
    if(){}elseif(){}else{}
    Condintion ? truepart; : elsepart; //can assign to variable
    Switch(variable){
        case:
            break;
    }

Console:

    console.log('message' or #+#)
        console.log(# , "" , #) //Can log more agruments

Conversion:

    Type Conversion:
        Number('')      //String to number
        String(#)       //Number to String
        Boolean:
            5 Falsy:
                - 0
                - ''
                - Undefined
                - Null
                - NaN
    Type Coercion:
        '#'+#+'#' - String
        '#'-#-'#' - Number
        '#'*#*'#' - Number
        '#'/#/'#' - Number

Functions:

    Declaration:
        function funcName( arg, arg,arg ){ return output; }
            funcName ( arg,arg ,arg );              //Called with
            variable = funcName( arg,arg ,arg );    //assigning to variable
    Expression
        variable = function (){return;}
            variable();
    Arrow Functions:
        funcName = parameter => code;                   //One lines
        funcName = parameter => {code; return output;}  //multiple lines
            funcName();

Arrays:

    const arrayName = [Value, value];           // Can be any type or combo: str, int, array
    const arrayName = new Array(value,value);   //different way
        arrayName[#];                           //To call a value at position
        arrayName[#] = newValue;                //Replaces value at position

    Methods:
        arrayName.length;               //Length of array
        arrayName.push(value);          //adding value to end, can push multiple values
        arrayName.unshift(value);       //adding value to front
        arrayName.pop();                //removes last value
        arrayName.shift();              //removes 1st value
        arrayName.indexOf(value);       //returns position of value
        arrayName.includes(value);      //returns Boolean if in array
        arrayName.concat(arrayName2);   //Merge arrays

Objects:

    const objectName = {key1: keyValue, key3:this.key1-2, key4: function(){} };   //like array but can assign keys but keyValue can be function expression, Can be any type or combo
        keyValue                        //can be function, prompt, boolean
        objectName.key                  //return keyValue
        objectName['key']               //return keyValue
        objectName.key = keyValue;      //creates new key with keyValue
        objectName['key'] = keyValue;   //creates new key with keyValue
    Methods:
        this                            //while in object this refers to object
        this.key;                       //return keyValue in object
        this.key = keyValue             //creates new key with keyValue in object

For Loops:

    for(let loopVar = startValue; loopVar < endValue; loopVar++){code}
        continue;           //skips to next loopVar
        break;              //stops loop
        for(){}             //Can make a loop in loop

While loop:

    while(loopVar < endValue){code}
        continue;           //skips to next loopVar
        break;              //stops loop
        for(){}             //Can make a loop in loop

DOM - Document Object Model:

    Is a WEB API    (Application Programming Interface)
    - const domElement = document.querySelector('element/.class/#id');  //Calls element
        domElement.textContent     //Calls text in element, can assign new text
        domElement.value           //Call value in input element, can assign new
        domElement.style.                   //Calling element style
                        .backgroundColour = '#colour'    //assigning colour  in string
                        .width = 'size'                 //assigning width in string
        domElement.addEventListener(eventType, listener, options)    //Adding listener
            Type:
                'click'     //Click on element
            Listener:
                function (){}   //Declared in the listener
                funcName        //Declared outside of listener
        domElement.appendChild(domNewElement)     //Add another element as child
        domElement.classList.
                            .remove('class/id')//Removes class,Type without the . or #
                            .add('class/id') //Add class to id, without the . or #
                            .contains('class/id')   //Checks for Class/ID
                            .toggle('class/id')     //adds and removes
        domElement.src = "NewScore" //Assigning Src
    - const domElement = document.getElementById('ID')  //Can use this for ID
    - const domElement = document.querySelectorAll('element/elementName'); //Calls elemts with same name, kinda like array
    - const domNewElement = document.createElement('typeofelement'); //Creates element
        domElement.appendChild(domNewElement)     //Add another element as child

    - document.addEventListener()    //Listens for anything

Math Object:

    Math.method
        Methods:
            .random()   //Returns random number between 0 to 1
            .trunc(x)   //Returns only integer
