# docker

## Run https on localhost

``` 
dotnet dev-certs https --trust (if not installed)
2.set ASPNETCORE_URLS=https://localhost:44360
3.dotnet run --no-launch-profile
```

## Set http proxy on current session 

### CMD

``` 
set http_proxy=http://ip:port
set https_proxy=http://ip:port
``` 

### Powershell

``` 
$env:http_proxy = "http://ip:port"
$env:https_proxy = "http://ip:port"
``` 

## Set a proxy on 

`docker build --build-arg http_proxy=http://ip:port --build-arg https_proxy=http://ip:port -t myawesomeimage:latest`

## delete all <none> images

`docker rmi $(docker images -f “dangling=true” -q)`


