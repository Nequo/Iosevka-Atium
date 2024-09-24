# Iosevka Spin

Custom Iosevka build.

## Building

First create the docker image to build in:
```
git clone --depth 1 https://github.com/be5invis/Iosevka.git
cd Iosevka/docker
docker build -t=fontcc .
```

Back in this repo, this will use private-build-plans.toml to build the ttf variants:
```
docker run -it --rm -v $PWD:/work fontcc ttf::IosevkaSpin
```
