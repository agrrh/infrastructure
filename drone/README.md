# Templates

This is a templated pipeline.

Usage:

```raw
drone template update \
  --namespace agrrh \
  --name pipeline.yaml \
  --data @drone/pipeline.yaml
```

Call it like this:

>Freeform params goes under `.data` object

```yaml
---

kind: template
load: pipeline.yaml
data:
  targets:
    - name: foo
    - name: bar
```
