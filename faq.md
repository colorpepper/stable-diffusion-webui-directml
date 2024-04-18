# problems when compiling
## windows environment
###  An HTTP error occurred when trying to retrieve this URL.
HTTP errors are often intermittent, and a simple retry will get you on your way.
SSLError(MaxRetryError('HTTPSConnectionPool(host=\'repo.anaconda.com\', port=443): Max retries exceeded with url: /pkgs/main/win-64/repodata.json.bz2

### solutions:
conda config --set ssl_verify false 







##linux environment
