### DON'T USE THESE PROXIES FOR SENSITIVE DATA!
#### Tested on Windows 10 / Python 3.9
##### pip install freeproxydownloader
<img src="https://github.com/hansalemaos/screenshots/raw/main/PROXY.png"/>



```python
 from freeproxydownloader import get_proxies
 get_proxies()
:param list_with_txt_file_links:
        Example
            ["https://raw.githubusercontent.com/TheSpeedX/SOCKS-List/master/socks5.txt",
            "https://raw.githubusercontent.com/TheSpeedX/SOCKS-List/master/socks4.txt",
            "https://raw.githubusercontent.com/TheSpeedX/PROXY-List/master/http.txt",
            "https://raw.githubusercontent.com/clarketm/proxy-list/master/proxy-list-raw.txt",
            "c:\\proxylist.txt"]
        (default=None) #Will choose randomly from list_with_txt_file_proxies
:param list_with_json_file_links:
        Example
            ["https://raw.githubusercontent.com/fate0/proxylist/master/proxy.list",
            "https://raw.githubusercontent.com/hookzof/socks5_list/master/tg/mtproto.json",
            "https://raw.githubusercontent.com/hookzof/socks5_list/master/tg/socks.json",]
        (default=None) #Will choose randomly from list_with_json_file_proxies

:param save_path_proxies_all_filtered:
        Folder for output
        (default=None) #Will create a folder in the root of your env, called "freeproxydownloader_results"

:param http_check_timeout:
        Timeout for http check with requests
        (default=10)

:param threads_httpcheck:
        How many threads when doing the http check with requests
        (default=20)

:param threads_ping:
        How many threads when doing the ping check
        (default=10)

:param silent:
        verbose or not
        (default=False)

:param max_proxies_to_check:
        stop checking after n checked proxies in total! (Not positive results!!)
        (default=False)

:return: filtered_proxies_xlsx, filtered_proxies_pkl #can be opened com pandas
```
