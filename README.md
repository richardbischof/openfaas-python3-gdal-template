# OpenFaaS Python3 GDAL Template  

A Python 3 with GDAL template for spatial operations in OpenFaaS.

## Downloading the template  
```   
faas template pull https://github.com/richardbischof/openfaas-python3-gdal-template
```   

## Using the python3-gdal template  

Create a new function  
```
faas new --lang python3-gdal <fn-name>  
```

Replace example gdal.VersionInfo() with your own logic.  
```
def handle(req):
    return gdal.VersionInfo()
```

Build, push and deploy  
```
faas up -f <fn-name>.yml
```

Execute function   
```
echo -n "<your-payload>" | faas invoke <fn-name> -
```

## Links
[OpenFaaS](https://www.openfaas.com/)
