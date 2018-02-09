# Common Metrix Stack Snapshot

You can use it in your Stack config to get a reproducible set of packages picked by Metrix instead of LTS or Nightly.

Following is an example of the `stack.yaml` file:

```yaml
resolver: https://raw.githubusercontent.com/metrix-ai/stack-snapshot/1/snapshot.yaml
packages:
extra-deps:
```

# Versioning

It is versioned using Git tags, making you capable of picking a snapshot by its version. Version is set in the `{version}` placeholder in the following URI:

```
https://raw.githubusercontent.com/metrix-ai/stack-snapshot/{version}/snapshot.yaml
```
