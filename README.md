# 01100111
01100111:01101000:01101111:01110011:01110100

## How to Use:

```
javascript:
function zero(l){
var z = [];
z[1] = document.createElement("script");
z[1].setAttribute("src","https://github.com/tinoni/translate.js");
z[0] = document.createElement("script");
z[0].setAttribute("src","https://code.jquery.com/jquery-3.3.1.js");
var b = document.getElementsByTagName("head");
for(var i = 0;i<b.length;i++){
  b[i].appendChild(z[i]);
};
var 
var d = {
  "Forums": {
    en: "Redtube"
  },
  "Download plugin": {
    en: "Download plugin"
  }
};
var t = $("body *").contents().filter(function(){
  return((this.nodeType == 3) && this.nodeValue.match(/\S/)); 
}).setAttribute("class","trn");
t.translate({lang:l,t:d});
return(t);
};
zero().lang("en");
```
