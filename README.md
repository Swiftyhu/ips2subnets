# ips2subnets
Perl script to help generate a shorter list from an IPv4 list, possibly using subnets.

# Example
```
cat <<<EOF | ./ips2subnets
127.0.0.1
127.0.0.4
127.0.0.2
127.0.0.3
10.0.0.128/25
10.0.0.0/25 
EOF
```

It will produce the following (shorter) output:
```
10.0.0.0/24
127.0.0.1
127.0.0.2/31
127.0.0.4
```
