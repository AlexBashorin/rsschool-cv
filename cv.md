# Alexandr Bashorin

### Contacts
* *Phone:* +7 (996) 218-60-87
* *Email:* bashorina5@gmail.com
* *Telegram:* @Alex_bash

### Summary
My main goal is to get a position as a front-end developer. Before taking part in this training, I worked as a graphic designer. In the spring, I started learning Figma, and also started learning JavaScript from a tutorial: https://learn.javascript.ru/.

### Skills
Basic knowledge of HTML, CSS, JavaScript.

### Latest code example
```javascript
function sudoku(puzzle) { 
  var sudoku=puzzle.map(x=>{return x.join("")}).join(",")  
  return next(sudoku).split(",").map(x=>{ return x.split("").map(z=>{return +z})})
}
function getPossibleDigits(row,column,str){
    var array=str.split(",")
    var hor=array[row]
    var ver=array.map(x=>{return x.charAt(column)})
    var sqrRow=Math.floor(row/3)*3
    var sqrColumn=Math.floor(column/3)*3    
    var sqr=[0,1,2].map(x=>{return array[sqrRow+x].substr(sqrColumn,3)}).join("")    
    return "123456789".replace(new RegExp("["+hor+ver+sqr+"]","g") ,"").split("")
}
function next(str){    
    var index = str.replace(/,/g,"").indexOf("0")
    if (index==-1) return str    
    var digits = getPossibleDigits(Math.floor(index/9),index%9,str)
    if (!digits[0]) return false 
    for (var i=0;i<digits.length; i++){      
      var temp = str.replace("0",digits[i])     
      var ch = next(temp)
      if(ch) return ch
    }    
}
```

### Experience


### Education
Udmurt state university

### English
Pre-intermediate
