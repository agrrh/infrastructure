# Servers

All servers are named. Names are generated through following pattern:

```
${NAME}${ID}.${LOCATION}.${DOMAIN}
```

| PART     | REGEXP                 | EXAMPLES |
| ---      | ---                    | --- |
| NAME     | `^[\w-]{3-32}$`        | `tmp`, `db`, `kube`, `bus-master` |
| ID       | `^[1-9][\d]*$`         | `1`, `99`, `101` |
| LOCATION | `^[\w][\d\w-]{2-15}$`  | `ru`, `us-north`, `aws-eu-west` |
| DOMAIN   | 2nd-level domain       | `example.com` |

Valid resulting examples are:

```
watson  1  . bakerst221b . detective.com
node    42 . narnia      . project.io
```
