# vscode-devcontainer-stackstorm

## Setup
### Create a link for specifying `ST2_PACKS_DEV`
```
$ ln -s ${PWD}/docker-compose.env ${PWD}/st2-docker/.env
```

## Development
### Register the pack
```
st2-docker-st2client-1# st2 run packs.load packs=<pack> register=all
```

### Create the virtualenv for pack
```
st2-docker-st2client-1# st2 run packs.setup_virtualenv packs=<pack>
```
