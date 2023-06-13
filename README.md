# Discord Server Joiner

Discord Server Joiner and Booster is a script that allows you to automatically join a Discord server using multiple user tokens. This script also supports server boosting and 2captcha API and Capmonster.cloud API key for captcha solving.

## Installation

Download [nodejs](https://nodejs.org/)



```
git clone https://github.com/erfgasergser/Discord-token-joiner
```



## Config

The config.json file contains the following properties:
- `captcha_service`: (optional) Your Captcha service (2Captcha or Capmonster)
- `captcha_api_key`: (optional) Your 2captcha or Capmonster API key for solving captchas.
- `inviteCode`: The invite code for the Discord server you wish to join.
- `joinDelay`: The delay (in milliseconds) between each join attempt.
- `useProxies`: Enable it if you want to use proxies (fill proxies in proxies.txt)
- `boost`: (optional) An object containing properties for server boosting.
    - `enabled`: Whether or not you want to boost the server on joining.
    - `delay`: The delay (in milliseconds) before boosting the server.
    - `serverId`: The ID of the server to boost.

### Program Usage

The program will automatically attempt to join the server using each token provided in the tokens.txt file. The `joinDelay` property determines the delay between each join attempt. 

When you open Discord-token-joiner.exe, it will start joining the server you specified. 


## Proxy Usage
If `useProxies` is enabled in the config, the program will use proxies from proxies.txt.
This program only supports `http` and `https` proxies.
proxies should be in the format `https://username:password@ip:port` if the proxy has authentication or `https://ip:port` if the proxy does not have authentication. 
NOTE: the http prefix is mandatory before the proxy 

### Error Handling

The program includes error handling for unhandled rejections and uncaught exceptions. If an error occurs, the program will log the error message and continue running.




## License
[MIT](https://choosealicense.com/licenses/mit/)
