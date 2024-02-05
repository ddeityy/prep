# String:

```go
type string struct {
    str unsafe.Pointer // pointer to first byte
	len int
}
```

```go
string := "привет"
for i, rune := range(string)
```

en = 1 bytes
ru = 2 bytes
ch = 3 bytes

# UTF-8 Encoding
1 bytes  0xxxxxxx
2 bytes  110xxxxx 10xxxxxx
3 bytes  1110xxxx 10xxxxxx 10xxxxxx
4 bytes  11110xxx 10xxxxxx 10xxxxxx 10xxxxxx
