# Serverless Functions

## Serverless Computing

[ibm.com](https://www.ibm.com/cloud/learn/serverless)

"Serverless is a cloud application model that lets developers build and run code without managing servers, and paying for idle cloud infastructure."

### Pros and cons of serverless

| Pros | Cons |
| ---- | ---- |
| Improved developer productivity | Unacceptable latency for certain applications |
| Pay for execution only | Higher costs for stable workloads |
| Develop in any language | Monitoring and debugging issues |
| Streamlined development cycle | Vendor lock in |
| Cost-efective performance |
| Usage visibility |

## Virtual Environments

[python.org](https://www.ibm.com/cloud/learn/serverless)

Creating virtual environments

`python3 -m venv /path/to/new/virtual/environment`

On windows invoke the venv command as follows:

`c:\>c:\Python35\python -m venv c:\path\to\myenv`

Activating the virtual environment

Windows:

| Shell | Command |
| ---- | ---- |
| cmd.exe | C:\> <venv>\Scripts\activate.bat |
| PowerShell | PS C:\> <venv>\Scripts\Activate.ps1

Everything else:

| Shell | Command |
| ---- | ---- |
| bash/zsh | $ source <venv>/vin/activate
| fish | $ source <venv>/bin/acitvate.fish |
| csh/tcsh | $ source <venv>/bin/activate.csh |
| PowerShell Core | PS C:\> <venv>\Scripts\Activate.ps1 |

## http.server

Example from [pymotw.com](https://pymotw.com/3/http.server/index.html) adding support for http and how to return a response to a client

```py
http_server_GET.py
from http.server import BaseHTTPRequestHandler
from urllib import parse


class GetHandler(BaseHTTPRequestHandler):

    def do_GET(self):
        parsed_path = parse.urlparse(self.path)
        message_parts = [
            'CLIENT VALUES:',
            'client_address={} ({})'.format(
                self.client_address,
                self.address_string()),
            'command={}'.format(self.command),
            'path={}'.format(self.path),
            'real path={}'.format(parsed_path.path),
            'query={}'.format(parsed_path.query),
            'request_version={}'.format(self.request_version),
            '',
            'SERVER VALUES:',
            'server_version={}'.format(self.server_version),
            'sys_version={}'.format(self.sys_version),
            'protocol_version={}'.format(self.protocol_version),
            '',
            'HEADERS RECEIVED:',
        ]
        for name, value in sorted(self.headers.items()):
            message_parts.append(
                '{}={}'.format(name, value.rstrip())
            )
        message_parts.append('')
        message = '\r\n'.join(message_parts)
        self.send_response(200)
        self.send_header('Content-Type',
                         'text/plain; charset=utf-8')
        self.end_headers()
        self.wfile.write(message.encode('utf-8'))


if __name__ == '__main__':
    from http.server import HTTPServer
    server = HTTPServer(('localhost', 8080), GetHandler)
    print('Starting server, use <Ctrl-C> to stop')
    server.serve_forever()
```

## API's

The library you need in python to enable you to consume API's is called requests

`python -m pip install requests`


Example of how to request data
```py
>>> import requests
>>> response = requests.get("https://randomuser.me/api/")
>>> response.text
```

## Things I want to learn more about

If we are about to use Python to gather data from an API instead of JavaScript how do you integrate that with JavaScript when building a website?