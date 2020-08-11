# javascript
function type(target){
    var ret =typeof(target);
    var template={
        "[object Array]":"array",
        "[object String]":"string-object",
        "[object Boolean]":"boolean-object",
        "[object Object]":"object",
        "[object Number]":"number-object"
    }
    if(target===null){
        return "null";
    }else if(ret=="object"){
        var str=Object.prototype.toString.call(target);
        return template[str];
    }else {return ret;}
}