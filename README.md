# CLI Sliding Puzzle Game

A command-line interface sliding puzzle game built with Python.

## Installation

To install the game, you need Python 3.7 or higher and pip. Then run:

pip install cli-sliding-puzzle

## Playing the Game

After installation, run the game by typing:

sliding-puzzle

Use arrow keys to move tiles. Press 'q' to quit.

## Development

### Setup

1. Clone the repository:
   git clone https://github.com/yourusername/cli-sliding-puzzle.git
   cd cli-sliding-puzzle

2. Create a virtual environment:
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

3. Install development dependencies:
   pip install build twine setuptools_scm

### Building and Publishing

1. Ensure all changes are committed to git.

2. List existing tags to determine the next version number:
   git tag --list

3. Create a new git tag for the version:
   git tag -a vX.X.X -m "Release version X.X.X"
   git push origin vX.X.X

4. Build the package:
   python -m build

5. Test the package locally:
   pip install dist/cli_sliding_puzzle-X.X.X-py3-none-any.whl

6. Upload to TestPyPI:
   twine upload --repository testpypi dist/*

7. If everything works, upload to PyPI:
   twine upload dist/*

## License

This project is licensed under the MIT License.
