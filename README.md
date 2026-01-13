BASED ON OPEN DUCK REFERENCE MOTION GENERATOR https://github.com/apirrone/Open_Duck_reference_motion_generator

![walk](https://github.com/rubieluo/bipedal_reference_motion/blob/main/simmed_walk.gif)

# Reference Motion Generator

Reference motion generator based on [Placo](https://github.com/Rhoban/placo).

> This repo uses `git-lfs`. Install it with `sudo apt install git-lfs` before cloning the repo

## Installation 

Install uv

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

## Usage

### Generate motions


```bash
uv run motion_generator/gait_playground.py 
```

In the playground, gaits can be adjusted/viewed until they are as desired. Every time a gait is run, a `dummy.json` file will be generated in the root folder. This contains frames that can be [replayed on the real robot](https://github.com/rubieluo/bipedal_sw). Every time a gait is run, it will overwrite the previous `dummy.json`, make sure to rename/move good gaits before rerunning. 
