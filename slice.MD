# Slice:

```go
type slice struct {
    array unsafe.Pointer // pointer to array
    len int
    cap int
}
```

```go
slice := append(slice, 1):
// (oldcap + 3 * 256) / 4
```