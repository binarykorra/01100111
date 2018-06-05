# 01100111
01100111:01101000:01101111:01110011:01110100

## How to Use:

```
javascript:
function zero(l){
var z = [];
var x = document.getElementsByTagName("*");
for(var c = 0;c<x.length;c++){
  x[c].classList.add("trn");
  console.log(x[c]);
};
z[1] = document.createElement("script");
z[1].setAttribute("src","https://github.com/tinoni/translate.js");
z[0] = document.createElement("script");
z[0].setAttribute("src","https://code.jquery.com/jquery-3.3.1.js");
var b = document.getElementsByTagName("head");
for(var i = 0;i<b.length;i++){
  b[i].appendChild(z[i]);
};
var d = {
  "Forums": {
    pt: "Pornhub"
  },
  "Download plugin": {
    pt: "Download plugin",
    fi: "Download plugin"
  }
};
var t = $("html").translate({lang:l,t:d}).lang("pt");
return(t);
};
zero("fi");
```
