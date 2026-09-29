# SSRF Test Markdown

## Image References

![IMDS](http://169.254.169.254/latest/meta-data/)
![localhost](http://localhost:8080/test.png)
![internal](http://192.168.1.1/admin)

## HTML in Markdown

<img src="http://169.254.169.254/latest/meta-data/iam/security-credentials/">
<iframe src="http://169.254.169.254/"></iframe>
<object data="http://169.254.169.254/latest/meta-data/"></object>
<embed src="http://169.254.169.254/latest/user-data">
<video src="http://169.254.169.254/"></video>
<audio src="http://169.254.169.254/"></audio>
<source src="http://169.254.169.254/">
<track src="http://169.254.169.254/">

## Link References

[IMDS Link](http://169.254.169.254/latest/meta-data/)

## CSS Reference

<style>
@import url("http://169.254.169.254/");
body { background: url("http://169.254.169.254/latest/meta-data/"); }
</style>
