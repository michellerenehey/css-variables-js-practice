# css-variables-js-practice
JS Day 3! 

# HTML 
- h2 header (with a span that holds a word with class"highlight")
- a div with a class of "controls" 
- in the div: three labels connected to three inputs: 
    1. spacing: 
        - label for"spacing"
        - input id"spacing" type"range" name"spacing" min"10" max"200" value"10" data-sizing"px"
    2. blur
        - label for"blur"
        - input id"blur" type"range" name"blur" min"10" max"200" value"10" data-sizing"px"
    3. base color 
        - label for"base"
        - input id"base" type"color" name"base" value"*pick a color*" 
- image 

# CSS
- create three variables in CSS: styling, base, and blur 
- use these variables on the image & the header
- using these on the inputs will be dynamic in JS! 

# JS
- grab the CSS variable by using querySelectorAll 
- loop through each of the variables in the nodeList (forEach), and add an event listener to each. first event listener: click; second event listener: mouseover. Seonc part of each: run a handleUpdate function.
- handleUpdate function: save this.dataset.sizing || '' to a variable. grab all CSS variables by using 'document.documentElement.style.setProperty(`--${this.name}`, this.value + variable from above)