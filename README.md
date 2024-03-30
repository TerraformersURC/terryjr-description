# Terry Jr. Description

Description package for Terry Jr. to simulate it using ROS, Gazebo and RViz.

## Setting up

### Cloning the repository

Clone this repository in the **source directory of your ROS workspace**.

```bash
git clone https://github.com/TerraformersURC/terryjr-description.git
```

> **Note:** Generate and use a Personal Access Token (PAT) in the place of password when prompted. Refer [here](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens) for more information.

With this, the package files are downloaded to your computer.

### Install dependencies

The shell script in the workspace template file handles the first-time setup
for this package but it's fairly straightforward to do it manually:

```bash
sudo apt update
rosdep update
rosdep install --from-paths src --ignore-src -r -y
```

The package manifest `package.xml` has the required dependencies listed.

Now the package on your computer is ready to build.

### Running the package

This package has launch files to view Terry Jr. in Gazebo and RViz.

Gazebo:

```bash
roslaunch terryjr_description gazebo.launch
```

RViz:

```bash
roslaunch terryjr_description display.launch
```

TODO: This package needs to be ported to ROS2 Humble.
