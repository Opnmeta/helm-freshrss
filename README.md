# helm-freshrss
## Overview
A Helm Chart for Freshrss. based on Official Docker image.
Freshrss support database SQLlite, Postgresql, MySQL. 
The Helm chart doesn't include database such as PostgresSQL or MySQL. if you need them, please prepare it the seperate chart. 
 
## TL;DR
1. update values.yaml persistence storage section (we use longhorn as default storageclass)
2. update values.yaml freshrss section 
3. update values.yaml ingress section(host:chart-example.local) 

```
helm upgrade --install freshrss ./freshrss -f values.yaml
```

