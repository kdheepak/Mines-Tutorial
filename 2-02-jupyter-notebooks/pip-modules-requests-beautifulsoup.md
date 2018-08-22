
### PIP

From the command line, you can run the following

```bash
pip install package_name
```

Try installing `beautifulsoup`

```bash
pip install beautifulsoup
```


```python
import bs4
```


```python
import requests
```


```python
url = "https://xkcd.com"
```


```python
response = requests.get(url)
```


    ---------------------------------------------------------------------------

    Error                                     Traceback (most recent call last)

    ~/miniconda3/lib/python3.6/site-packages/urllib3/contrib/pyopenssl.py in wrap_socket(self, sock, server_side, do_handshake_on_connect, suppress_ragged_eofs, server_hostname)
        440             try:
    --> 441                 cnx.do_handshake()
        442             except OpenSSL.SSL.WantReadError:


    ~/miniconda3/lib/python3.6/site-packages/OpenSSL/SSL.py in do_handshake(self)
       1805         result = _lib.SSL_do_handshake(self._ssl)
    -> 1806         self._raise_ssl_error(self._ssl, result)
       1807


    ~/miniconda3/lib/python3.6/site-packages/OpenSSL/SSL.py in _raise_ssl_error(self, ssl, result)
       1545         else:
    -> 1546             _raise_current_error()
       1547


    ~/miniconda3/lib/python3.6/site-packages/OpenSSL/_util.py in exception_from_error_queue(exception_type)
         53
    ---> 54     raise exception_type(errors)
         55


    Error: [('SSL routines', 'ssl3_get_server_certificate', 'certificate verify failed')]


    During handling of the above exception, another exception occurred:


    SSLError                                  Traceback (most recent call last)

    ~/miniconda3/lib/python3.6/site-packages/urllib3/connectionpool.py in urlopen(self, method, url, body, headers, retries, redirect, assert_same_host, timeout, pool_timeout, release_conn, chunked, body_pos, **response_kw)
        600                                                   body=body, headers=headers,
    --> 601                                                   chunked=chunked)
        602


    ~/miniconda3/lib/python3.6/site-packages/urllib3/connectionpool.py in _make_request(self, conn, method, url, timeout, chunked, **httplib_request_kw)
        345         try:
    --> 346             self._validate_conn(conn)
        347         except (SocketTimeout, BaseSSLError) as e:


    ~/miniconda3/lib/python3.6/site-packages/urllib3/connectionpool.py in _validate_conn(self, conn)
        849         if not getattr(conn, 'sock', None):  # AppEngine might not have  `.sock`
    --> 850             conn.connect()
        851


    ~/miniconda3/lib/python3.6/site-packages/urllib3/connection.py in connect(self)
        325             server_hostname=hostname,
    --> 326             ssl_context=context)
        327


    ~/miniconda3/lib/python3.6/site-packages/urllib3/util/ssl_.py in ssl_wrap_socket(sock, keyfile, certfile, cert_reqs, ca_certs, server_hostname, ssl_version, ciphers, ssl_context, ca_cert_dir)
        328     if HAS_SNI:  # Platform-specific: OpenSSL with enabled SNI
    --> 329         return context.wrap_socket(sock, server_hostname=server_hostname)
        330


    ~/miniconda3/lib/python3.6/site-packages/urllib3/contrib/pyopenssl.py in wrap_socket(self, sock, server_side, do_handshake_on_connect, suppress_ragged_eofs, server_hostname)
        447             except OpenSSL.SSL.Error as e:
    --> 448                 raise ssl.SSLError('bad handshake: %r' % e)
        449             break


    SSLError: ("bad handshake: Error([('SSL routines', 'ssl3_get_server_certificate', 'certificate verify failed')],)",)


    During handling of the above exception, another exception occurred:


    MaxRetryError                             Traceback (most recent call last)

    ~/miniconda3/lib/python3.6/site-packages/requests/adapters.py in send(self, request, stream, timeout, verify, cert, proxies)
        439                     retries=self.max_retries,
    --> 440                     timeout=timeout
        441                 )


    ~/miniconda3/lib/python3.6/site-packages/urllib3/connectionpool.py in urlopen(self, method, url, body, headers, retries, redirect, assert_same_host, timeout, pool_timeout, release_conn, chunked, body_pos, **response_kw)
        638             retries = retries.increment(method, url, error=e, _pool=self,
    --> 639                                         _stacktrace=sys.exc_info()[2])
        640             retries.sleep()


    ~/miniconda3/lib/python3.6/site-packages/urllib3/util/retry.py in increment(self, method, url, response, error, _pool, _stacktrace)
        387         if new_retry.is_exhausted():
    --> 388             raise MaxRetryError(_pool, url, error or ResponseError(cause))
        389


    MaxRetryError: HTTPSConnectionPool(host='xkcd.com', port=443): Max retries exceeded with url: / (Caused by SSLError(SSLError("bad handshake: Error([('SSL routines', 'ssl3_get_server_certificate', 'certificate verify failed')],)",),))


    During handling of the above exception, another exception occurred:


    SSLError                                  Traceback (most recent call last)

    <ipython-input-4-237b9c36258c> in <module>()
    ----> 1 response = requests.get(url)


    ~/miniconda3/lib/python3.6/site-packages/requests/api.py in get(url, params, **kwargs)
         70
         71     kwargs.setdefault('allow_redirects', True)
    ---> 72     return request('get', url, params=params, **kwargs)
         73
         74


    ~/miniconda3/lib/python3.6/site-packages/requests/api.py in request(method, url, **kwargs)
         56     # cases, and look like a memory leak in others.
         57     with sessions.Session() as session:
    ---> 58         return session.request(method=method, url=url, **kwargs)
         59
         60


    ~/miniconda3/lib/python3.6/site-packages/requests/sessions.py in request(self, method, url, params, data, headers, cookies, files, auth, timeout, allow_redirects, proxies, hooks, stream, verify, cert, json)
        506         }
        507         send_kwargs.update(settings)
    --> 508         resp = self.send(prep, **send_kwargs)
        509
        510         return resp


    ~/miniconda3/lib/python3.6/site-packages/requests/sessions.py in send(self, request, **kwargs)
        616
        617         # Send the request
    --> 618         r = adapter.send(request, **kwargs)
        619
        620         # Total elapsed time of the request (approximately)


    ~/miniconda3/lib/python3.6/site-packages/requests/adapters.py in send(self, request, stream, timeout, verify, cert, proxies)
        504             if isinstance(e.reason, _SSLError):
        505                 # This branch is for urllib3 v1.22 and later.
    --> 506                 raise SSLError(e, request=request)
        507
        508             raise ConnectionError(e, request=request)


    SSLError: HTTPSConnectionPool(host='xkcd.com', port=443): Max retries exceeded with url: / (Caused by SSLError(SSLError("bad handshake: Error([('SSL routines', 'ssl3_get_server_certificate', 'certificate verify failed')],)",),))



```python
soup = bs4.BeautifulSoup(response.content, "lxml")
```


```python
soup
```
