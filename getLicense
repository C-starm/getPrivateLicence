import requests
import json

session = requests.session()

burp0_url = "http://vrg123.com:80/loadcode/"
burp0_cookies = {"csrftoken": "7Y28BdVzNst0BNg8DMAVLR7wBqlANC2KHxYoi5cg35wzH70phXDm5zqJnCdQlWbe"}
burp0_headers = {"Accept": "*/*", "X-CSRFToken": "7Y28BdVzNst0BNg8DMAVLR7wBqlANC2KHxYoi5cg35wzH70phXDm5zqJnCdQlWbe", "X-Requested-With": "XMLHttpRequest", "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 11_2_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36", "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8", "Origin": "http://vrg123.com", "Referer": "http://vrg123.com/", "Accept-Encoding": "gzip, deflate", "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8", "Connection": "close"}
burp0_data = {"password": "6575"}
response = session.post(burp0_url, headers=burp0_headers, cookies=burp0_cookies, data=burp0_data)
print(json.loads(response.text)['codeval'])
