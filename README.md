## WIP

Headlamp Flux (testing)

### Known Issues

* On OpenShift, the securityContext.runAsUser must be set to null
  * It is difficult to patch a "null" into helmrelease values
  * (The methods I've tried so far did not work)

You wind up with:

```yaml
spec:
  values:
    securityContext: {}
```

(which is incorrect, we want to see)

```yaml
spec:
  values:
    securityContext:
      runAsUser: ~
      runAsGroup: ~
```

