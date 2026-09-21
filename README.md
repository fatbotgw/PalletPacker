# Pallet Packer
This purpose of this program is to calculate the optimal loading pattern
and maximum quantity of pallets that can be loaded into a semi trailer
or shipping container.  The pallets are not "a single pallet with many boxes",
but are stacks of identical pallets.

## Motivation
This is a personal project created for [Boot.dev](https://www.boot.dev). 
It is based on a pain point I experienced at a former employer.


## Quick Start
### Requirements
* Python >= 3.13
* uv
* textual (pulled in by uv)
* pint (pulled in by uv)

### Steps
1) clone the clode
2) ```uv run src/main.py```
3) follow the prompts

## Usage
After starting the program, you will be greeted by a prompt asking for container
size.  The available choices are listed, pick the one you want.

Next, pick the pallet model.  In this case, you'll need to see which ones are
listed in the ```constants.py``` file.  Only a subset of pallets were added.

The program will then calculate the total amount of pallets (in stacks) that
can fit in the chosen container size. The output also includes the preferred
orientation for placement. For that, "L" is the pallet's longest side in a front-to-back orientation related to the container. And "W" is the pallet's
longest side in a side-to-side orientation related to the container.