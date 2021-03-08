# launch_debug_ws

Debug Workspace for ros2 launch

## Usage

```sh
git clone git@github.com:kenji-miyake/launch_debug_ws.git
cd missing_noetic_pkgs
mkdir -p src
vcs import src < workspace.repos
colcon build --symlink-install --cmake-args -DCMAKE_BUILD_TYPE=Release
```

You need to sed environment variables before using this workspace.

```sh
export LAUNCH_DEBUG_WORKSPACE=PATH_TO_YOUR_WORKSPACE
export LAUNCH_DEBUG_LAUNCH=PATH_TO_YOUR_LAUNCH
```

Then, open VSCode and press F5 to start debugging!
