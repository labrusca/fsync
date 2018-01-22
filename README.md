Package `fsync` keeps files and directories in sync. 

fork&modify from
[fsync](https://github.com/mostafah/fsync).

![demo](https://github.com/labrusca/fsync/images/show.gif)

 Add ```Syncer.Output bool```:
```
type Syncer struct {
	// Set this to true to delete files in the destination that don't exist
	// in the source.
	Delete bool
	// By default, modification times are synced. This can be turned off by
	// setting this to true.
	NoTimes bool
	// Output each file name during sync.
	Output bool
	// TODO add options for not checking content for equality
}
```

---
#### MIT Licsence