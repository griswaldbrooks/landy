# landy
Landmark based localization library

# Development Container
Build a new development image
```shell
mkdir -p ~/.landy/ccache
export UID=$(id -u) export GID=$(id -g); docker compose -f compose.dev.yml build
```
Start an interactive development container
```shell
docker compose -f compose.dev.yml run development
```
Build the repository in the container
```shell
cmake -S src/landy/ -B build
cmake --build build
```

# Run
```shell
username@landy-dev:~/ws$ ./build/landy_example
```
