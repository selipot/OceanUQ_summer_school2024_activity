This repository is for educational purposes and the material is currently incomplete and not ready to be used: please check back later this summer for the final (ready to use) version!

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/donatagiglio/OceanUQ_summer_school2024_activity/HEAD)

## Running with Docker

Create a free Docker account at https://www.docker.com/ and install Docker (https://www.docker.com/products/docker-desktop/) on your laptop. Check that git is also installed on your laptop. Before moving forward, please make sure no other jupyter notebooks are running on your laptop. With Docker installed (and running) on your laptop clone the `https://github.com/donatagiglio/OceanUQ_summer_school2024_activity/` repo, change directory into it, and mount it into a containerized environment:

```
git clone https://github.com/donatagiglio/OceanUQ_summer_school2024_activity
cd OceanUQ_summer_school2024_activity
docker container run -p 8888:8888 -v $(pwd):/books argovis/notebooks:OceanUQ2024
```

After a moment, several URLs will be printed to the terminal. Copy the one beginning with http://127.0.0.1 to your browser of choice to access the notebook environment.

## Edits to the above, if you are using Windows
Once you have cloned the demo_notebooks repository:
- use `Windows powershell` to `cd` to the `demo_notebooks` directory
- use `Windows powershell` to run the this command:

  ```
  docker container run -p 8888:8888 -v path_to_files:/books argovis/notebooks:OceanUQ2024 jupyter notebook --allow-root --ip=0.0.0.0
  ```

  Please note that `path_to_files` is the full path to the `OceanUQ_summer_school2024_activity` directory on your machine, e.g. `C:\Users\username\python_files\OceanUQ2024\OceanUQ_summer_school2024_activity`.
- After a moment, several URLs will be printed to the terminal. Copy the one beginning with http://127.0.0.1 to your browser of choice to access the notebook environment. 
