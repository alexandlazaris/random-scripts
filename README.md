# random-scripts
Random scripts I use for ad-hoc tasks


## Rename .HEIC to .PNG

Useful after sharing photos from an iphone to a desktop and wanting a compatible file extension. 

> [!NOTE]
> I should also add error handling & counting in here, make a pretty log output too.

```
# bin/sh

for file in *.HEIC; do
    echo $file
    mv -- "$file" "${file%.HEIC}.PNG"
done
```
