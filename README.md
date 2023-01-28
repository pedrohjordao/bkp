THIS IS A WORK IN PROGRESS

# An Exceedingly Simple File Mover

Do you often create backup of config files? This tool is for you.

## Usage

The simplest usage example is

```
$ bkp my_file
```

This will move `my_file` and rename it to `my_file.bkp`.

But the tool is more powerful

```
$ bkp --interative --extension backup --output ~/backup -r --keep-structure *.yaml 
```

This will:

1. Go through every file with the `.yaml` extension recursively from the current directory
2. Move them to `~/backup`
3. Add the `backup` extension

And do it all interactively, asking for confirmation in each file
