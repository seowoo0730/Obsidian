## Object → JSON `stringify`

```JavaScript
const user1 = {
  name: `Mike`,
  age: 14,
  birthDate: new Date(),
};

let json = JSON.stringify(user1);
console.log(json); //{"name":"Mike","age":14,"birthDate":"2022-03-30T12:10:07.125Z"}
```

## JSON → Object `parse`

```JavaScript
const user1 = {
  name: `Mike`,
  age: 14,
  birthDate: new Date(),
};

let json = JSON.stringify(user1);
const obj = JSON.parse(json);
console.log(obj); //{name: 'Mike', age: 14, birthDate: '2022-03-30T12:15:09.095Z'}
```

> [!info] JSON Diff  
> Validate, format, and compare two JSON documents.  
> [http://jsondiff.com/](http://jsondiff.com/)  

> [!info] Json Beautifier - Json Formatter | Json Viewer | Json Editor  
> JSON Beautifier helps to perform below tasks: It also provides different types of view (like code, tree, form, view, text, preview) which helps to Display data as you want.  
> [https://jsonbeautifier.org/](https://jsonbeautifier.org/)  

> [!info] JSON Parser - Best JSON Formatter | JSON Editor  
> JSON Parser is used to format your JSON data into a properly readable JSON Format.  
> [https://jsonparser.org/](https://jsonparser.org/)