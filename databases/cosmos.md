### Count records in a collection
```
SELECT value count(1) FROM c
```

### Query collection without a property OR at specific value
```cosmos
where (c.color = @color OR NOT IS_DEFINED(c.color))
```