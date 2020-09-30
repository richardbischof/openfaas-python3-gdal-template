# OpenFaaS Python3 GDAL Template  

A Python 3 with GDAL template for spatial operations in OpenFaaS.

## Downloading the template  
`   
faas template pull https://github.com/richardbischof/openfaas-python3-gdal-template
`   

## Using the python3-gdal template  

Create a new function  
`  
faas new --lang python3-gdal <fn-name>  
` 

Build, push and deploy  
`  
faas up -f <fn-name>.yml
`

Execute
`
echo -n "" | faas invoke <fn-name> -
`