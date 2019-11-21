Provide small but useful shell scripts to report status in startup scripts.

## Exemple:

```bash
echo -n "- Starting something..."
command_to_start_something > logfile
if (( $? == 0 ))
then
    echo_ok
else
    echo_nok
    exit 1
fi
```

## Install:

### From repository

```bash
autoreconf --install
./configure
make install
```

### From source archive

```bash
./configure
make install
```
