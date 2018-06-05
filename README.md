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
  console.log(z[i] + " loaded..");
  b[i].appendChild(z[i]);
};
var d = {
  "Forums": {
    zx: translator.get("Forums")
  },
  "Download plugin": {
    zx: "Download plugin",
    fi: "Download plugin"
  }
};
console.log(translator.get("Forums"));
var t = $("html").translate({lang:l,t:d}).lang("zx");
return(t);
};
zero("fi");
```
