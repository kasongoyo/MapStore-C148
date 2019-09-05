Photomap
==========

Quick Start
------------

Clone the repository with the --recursive option to automatically clone submodules:

`git clone --recursive https://github.com/geosolutions-it/MapStore-C148`

Install NodeJS >= 7.10.0 , if needed, from [here](https://nodejs.org/en/download/releases/).

Start the development application locally:

`npm install`

`npm start`

The application runs at `http://localhost:8081` afterwards.

Read more on the [wiki](https://github.com/geosolutions-it/MapStore-C148/wiki).

Themes
------------
This project support two themes, the default theme which is used by default and another theme called `surveye theme`. Please refer to [Mapstore theme guide](https://mapstore.readthedocs.io/en/latest/developer-guide/customize-theme/) on how to use surveye theme during development and refer to build section below on how to build with a theme.

Build
----------------

This project use maven as the build tool, it uses `build.sh` script to automate the build process. To build run  

`$ sh build.sh`     

The maven build include two profiles, the **default profile** and **surveye profile**. To build surveye profile,
just provide theme command line argument as follows;   

`$ sh build theme="surveye"`

Default profile is activated when no `theme` argument or invalid theme argument is provided. You can also provide mapstore
version to be used during the build by providing `version` argument to the build script as follows;

`$ sh build version='SNAPSHOT-2019'`