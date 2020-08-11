数组去重
var arr=[1,1,1,1,2,2,2,3,3,3,4,4];
Array.prototype.unique=function(){
    var temp={},
        arr=[],
        len=this.length;
        for(var i=0;i<len;i++){
            if(!temp[this[i]]){
                temp[this[i]]='abc';
                arr.push(this[i]);
            }
        }
        return arr;
}