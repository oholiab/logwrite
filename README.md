Logwrite
================================

Logwrite is a simple wrapper for a logger instance to turn it in to
a filehandle-type object that can be used to redirect $sterr and
$stdout, for instance:

```ruby
$log = Logger.new("/var/log/somelog")
$stderr = Logwrite.new($log, "stderr")
$stdout = Logwrite.new($log, "stdout")
```

Possibly unnecessary or missing some really important feature, pull requests accepted gracefully.
