# Check whether the namespace exist
## bash/shell

```bash
if ! kubectl get namespaces -o json | jq -r ".items[].metadata.name" | grep staging;then
  echo 'HALLO'
fi
```
