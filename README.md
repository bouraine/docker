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


