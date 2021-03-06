[![Build Status](https://travis-ci.org/rhenning/x509_sleuth.svg?branch=master)](https://travis-ci.org/rhenning/x509_sleuth)

# x509_sleuth

A tool to remotely scan for and investigate X.509 certificates used in SSL/TLS

# Usage

Clone this repo
```
cd x509_sleuth
bundle install
bundle exec rake install
cd examples
bundle install
bundle exec ./example.rb
```
You should see output similar to:

```
+----------------+--------------------------------------------------------------------+---------------------+-------------------------+-------------------------+
| host           | subject                                                            | serial              | not_before              | not_after               |
+----------------+--------------------------------------------------------------------+---------------------+-------------------------+-------------------------+
| www.google.com | /C=US/ST=California/L=Mountain View/O=Google Inc/CN=www.google.com | 5727081030881357105 | 2015-01-14 13:14:16 UTC | 2015-04-14 00:00:00 UTC |
+----------------+--------------------------------------------------------------------+---------------------+-------------------------+-------------------------+
```

# Contributors

* [Richard Henning](https://github.com/rhenning)
* [Travis Truman](https://github.com/trumant)
