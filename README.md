# 01100111
01100111:01101000:01101111:01110011:01110100

## How to Use:

```
javascript:
function zero(language){
var z = [];
z[1] = document.createElement("script");
z[1].setAttribute("src","https://github.com/tinoni/translate.js");
z[0] = document.createElement("script");
z[0].setAttribute("src","https://code.jquery.com/jquery-3.3.1.js");
var b = document.getElementsByTagName("head");
for(var i = 0;i<b.length;i++){
  b[i].appendChild(z[i]);
};
var dict = {
  "Google": {
    en: "Google",
    fi: "Pornhub"
  }
  "Google": {
    en: "Google",
    fi: "Youjizz"
  }
};
var h = $("body");
var t = h.translate({lang:language,t:dict});
return(t);
};
zero().lang("fi");
```
