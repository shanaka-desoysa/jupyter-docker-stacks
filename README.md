# Jupyter Docker Stacks

This repo contains a easy-to configure jupyter notebook that runs from a `docker-compose`. See the [jupyter-docker-stacks documentation](https://jupyter-docker-stacks.readthedocs.io/en/latest/)


## Run

All you need to do is use the regulare docker-compose command:

```
docker-compose up -d
```

## Stop

```
docker-compose down

```

## Access

This is the default location of the notebook:

```
http://127.0.0.1:8888/
```

The defualt password is `6a833e4b32233ab6`

In order to make the container publicly available, edit `docker-compose.yaml` and replace `- "127.0.0.1:8888:8888"` 
with `- "8888:8888"`.

##  Configure

The config files are located in `./config` folder, edit the `jupyter-config.json` for customization.