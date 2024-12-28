# Iosevka Atium

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
docker run -it --rm -v $PWD:/work fontcc ttf::IosevkaAtium
```

## Screenshot

<img width="220" alt="image" src="https://github.com/user-attachments/assets/89cc01e0-c66d-475f-b3ce-5fcf35fb808b" />
