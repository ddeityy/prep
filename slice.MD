# Slice:

```go
type slice struct {
    array unsafe.Pointer // pointer to array
    len int
    cap int
}
```

## Append

(oldcap + 3 * 256) / 4