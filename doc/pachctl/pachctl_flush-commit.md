## ./pachctl flush-commit

Wait for all commits caused by the specified commits to finish and return them.

### Synopsis


Wait for all commits caused by the specified commits to finish and return them.

Examples:

	# return commits caused by foo/abc123 and bar/def456
	$ pachctl flush-commit foo/abc123 bar/def456

	# return commits caused by foo/abc123 leading to repos bar and baz
	$ pachctl flush-commit foo/abc123 -r bar -r baz



```
./pachctl flush-commit commit [commit ...]
```

### Options

```
  -r, --repos value   Wait only for commits leading to a specific set of repos (default [])
```

### Options inherited from parent commands

```
      --log-flush-frequency duration   Maximum number of seconds between log flushes (default 5s)
  -v, --verbose                        Output verbose logs
```

### SEE ALSO
* [./pachctl](./pachctl.md)	 - 

###### Auto generated by spf13/cobra on 12-Sep-2016