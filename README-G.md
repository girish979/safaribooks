## Accessing through a SSO Login
Login to safari and then to go profile page

run below code in browser console pressing f12. copy the output as to file `cookies.json` and copy it in root folder
```
copy(JSON.stringify(document.cookie.split(';').map(c => c.split('=')).map(i => [i[0].trim(), i[1].trim()]).reduce((r, i) => {
    r[i[0]] = i[1];
    return r;
}, {})))

```

