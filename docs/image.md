## Delete image

```js
    client.image(fingerprint)
        .then( (image) => {
            image.delete()
                .then( () => console.log("successfully removed") )
                .catch( (err) => console.log(err))
        } )
        .catch( (err) => console.log(err) )
```


## Fetch all images
```js

bool lazy;

const images = await client.images(lazy);

```

in case of lazy fetching are just metadata returned
