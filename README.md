# 01100111
01100111:01101000:01101111:01110011:01110100

## How to Use:

```
javascript:
(function($){
  $.fn.translate = function(options) {
    var that = this;
    var settings = {
      css: "trn",
      lang: "en"
    };
    settings = $.extend(settings, options || {});
    if (settings.css.lastIndexOf(".", 0) !== 0)
      settings.css = "." + settings.css;  
    var t = settings.t;
    this.lang = function(l) {
      if (l) {
        settings.lang = l;
        this.translate(settings);
      }        
      return settings.lang;
    };
    this.get = function(index) {
      var res = index;
      try {
        res = t[index][settings.lang];
      }
      catch (err) {
        return index;
      }
      if (res)
        return res;
      else
        return index;
    };
    this.g = this.get;
    this.find(settings.css).each(function(i) {
      var $this = $(this);
      var trn_key = $this.attr("data-trn-key");
      if (!trn_key) {
        trn_key = $this.html();
        $this.attr("data-trn-key", trn_key);
      }
      $this.html(that.get(trn_key));
    });
		return this;
  };
})(jQuery);
function zero(l){
var z = [];
var x = document.getElementsByTagName("*");
for(var c = 0;c<x.length;c++){
  x[c].classList.add("trn");
  x[c].setAttribute("data-trn-key",x[c].innerHTML);
  console.log(x[c]);
};
z[0] = document.createElement("script");
z[0].setAttribute("src","https://code.jquery.com/jquery-3.3.1.js");
z[1] = document.createElement("script");
z[1].setAttribute("src","https://raw.githubusercontent.com/tinoni/translate.js/master/jquery.translate.js");
for(var i = 0;i<z.length;i++){
  console.log(z[i] + " loaded..");
  document.getElementsByTagName("head")[0].appendChild(z[i]);
};
var d = {
  "Forums": {
    pt: "Pornhub",
    en: "Pornhub"
  }
};
var t = $("body").translate({lang:l,t:d});
return(t);
};
zero("en");
```
