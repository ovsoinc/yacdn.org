# yacdn.org
Yet Another CDN.

[![Build Status](https://travis-ci.org/ovsoinc/yacdn.org.svg?branch=master)](https://travis-ci.org/ovsoinc/yacdn.org)
[![Coverage Status](https://coveralls.io/repos/github/ovsoinc/yacdn.org/badge.svg?branch=master)](https://coveralls.io/github/ovsoinc/yacdn.org?branch=master)
[![License](https://img.shields.io/badge/license-AGPLv3-blue.svg?label=license)](https://github.com/Storj/ovsoinc/yacdn.org/blob/master/LICENSE)
[![CDN Hits](https://img.shields.io/badge/dynamic/json.svg?label=CDN%20Hits&url=https://yacdn.org/stats&query=$.cdnHits&colorB=green)](https://img.shields.io/badge/dynamic/json.svg?label=CDN%20Hits&url=https://yacdn.org/stats&query=$.cdnHits&colorB=green)
[![Proxy Hits](https://img.shields.io/badge/dynamic/json.svg?label=Proxy%20Hits&url=https://yacdn.org/stats&query=$.proxyHits&colorB=green)](https://img.shields.io/badge/dynamic/json.svg?label=Proxy%20Hits&url=https://yacdn.org/stats&query=$.proxyHits&colorB=green)

## CDN

#### How to Use
```
https://yacdn.org/serve/<uri>
```

#### Example
```
https://yacdn.org/serve/http://meowbaari.com/wp-content/uploads/2016/06/1464933654_cat_sleep.png
```
![https://yacdn.org/serve/http://meowbaari.com/wp-content/uploads/2016/06/1464933654_cat_sleep.png](https://yacdn.org/serve/http://meowbaari.com/wp-content/uploads/2016/06/1464933654_cat_sleep.png)

#### Embeddable Script
Paste this into your browser console to replace all images.
```html
<script>
document.addEventListener('ready', function() {
    var imgs = document.getElementsByTagName("img");
    for (var i = 0, l = imgs.length; i < l; i++) {
        imgs[i].src = `https://yacdn.org/serve/${imgs[i].src}`;
    }
});
</script>
```

## Proxy

#### How to Use
```
https://yacdn.org/proxy/<uri>
```

#### Example
```
https://yacdn.org/proxy/http://meowbaari.com/wp-content/uploads/2016/06/1464933927_cat_acrobat.png
```
![https://yacdn.org/proxy/http://meowbaari.com/wp-content/uploads/2016/06/1464933927_cat_acrobat.png](https://yacdn.org/proxy/http://meowbaari.com/wp-content/uploads/2016/06/1464933927_cat_acrobat.png)
