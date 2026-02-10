
# Minejourney

A machine-learning powered Minecraft build generator. It takes simple text prompts and turns them into downloadable `.schem` files, allowing players to paste AI-generated structures straight into their Minecraft worlds.

## Features
- Generate Minecraft structures from text prompts
- Export builds as `.schem` files
- Visualize and process Minecraft schematics as voxel tensors
- Train and use 3D convolutional neural networks for structure generation

## Setup Instructions

1. **Clone the repository:**
	```sh
	git clone https://github.com/JamesDillonDev/minejourney.git
	cd minejourney
	```

2. **Create a virtual environment:**
	```sh
	python -m venv .venv
	```

3. **Activate the virtual environment:**
	- On Windows:
	  ```sh
	  .venv\Scripts\activate
	  ```
	- On macOS/Linux:
	  ```sh
	  source .venv/bin/activate
	  ```

4. **Install dependencies:**
	```sh
	pip install -r requirements.txt
	```
	Or, manually install the main packages:
	```sh
	pip install nbtlib matplotlib torch numpy
	```

## Usage

1. **Prepare your schematic files:**
	- Place `.schem` files in the `dataset/` folder.

2. **Open the Jupyter notebook:**
	```sh
	jupyter notebook 01_schematic_to_voxel.ipynb
	```

3. **Run the notebook cells:**
	- The notebook will process schematics, train a model, and generate new structures.

4. **Export generated builds:**
	- Generated voxel data can be exported as `.schem` files for use in Minecraft.

## Dependencies
- Python 3.8+
- nbtlib
- matplotlib
- torch
- numpy

## Virtual Environment
This project uses a Python virtual environment. The `.venv/`, `Lib/`, `Include/`, and `Scripts/` folders are excluded from version control via `.gitignore`.

To activate the environment each time you work on the project:
```sh
source .venv/bin/activate  # or .venv\Scripts\activate on Windows
```

## License
See [LICENSE](LICENSE) for details.
