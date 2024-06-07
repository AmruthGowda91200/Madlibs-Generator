
# Mad Libs Generator

The Mad Libs Generator is a fun Python project that allows users to create personalized stories by filling in placeholders with their own words. The script reads a template story with placeholders from a file and prompts the user for inputs to replace these placeholders, resulting in a unique story each time.



## Table of Contents

Features  
Requirements  
Installation  
Usage  
Example Outputs   
How It Works  
Customization  
Contributing  
License  
## Features 
* Reads story templates with placeholders from a file.  
* Prompts users for various words to fill in the placeholders.  
* Replaces placeholders with user inputs to create a customized story.  
* Supports a variety of placeholder types such as <noun>, <adjective>, <place>, etc.  
* Outputs the final story with the user's inputs.
## Requirements

* Python 3.x  
* A text file containing the story template (e.g., `story.txt`)
## Installation

1. Clone the Repository:
```bash
  git clone https://github.com/AmruthGowda91200/mad-libs-generator.git
```

2. Navigate to the Project Directory:
    ```bash
    cd mad-libs-generator
    ```

3. Ensure Python 3.x is Installed:

    ```bash
    python3 --version
    ```
## Usage

1. Create a Story Template:

* Create a file named story.txt in the project directory.
* Add a story with placeholders in the following format:

```txt
In the land of <place>, a <adjective> <noun> named <name> decided to explore the <adjective> <fantasy_place>. With a <adjective> <object> and a <adjective> <noun>, <name> ventured into the <adjective> forest.

```

2. Run the Script:

```bash
python3 madlibs_generator.py

```

3. Follow the Prompts:

* The script will prompt you to enter words for each placeholder.
* Type in your responses and press Enter.

4. View the Customized Story:

* After entering all required words, the script will display the completed story.


Example Command:

```bash
python3 madlibs_generator.py

```

Example Prompt:

```bash
Enter a word for <place>: Wonderland
Enter a word for <adjective>: magical
Enter a word for <noun>: explorer
Enter a word for <name>: Alice
...

```

Example Story Output:

``` bash 
In the land of Wonderland, a magical explorer named Alice decided to explore the magical Enchanted Forest. With a magical map and a magical backpack, Alice ventured into the magical forest.
...

```


## How It Works

The script reads the content of `story.txt`, identifies placeholders within `<` and `>`, prompts the user for words corresponding to these placeholders, and replaces them in the story to generate a customized output. Here’s a step-by-step breakdown:

1. Reading the Story:

```python 
with open("story.txt", "r") as f:
    story = f.read()
```

2. Finding Placeholders:

* It scans the story for words within < and >.
* Extracts and stores unique placeholders in a set.
3. Prompting User:

* Asks the user to input words for each placeholder.
* Stores these inputs in a dictionary.
4. Replacing Placeholders:

* Replaces each placeholder in the story with the corresponding user input.
* Outputs the final customized story.
## Customization

You can customize the Mad Libs generator by:

* Changing the Story Template: Edit `story.txt` with different placeholders and story content.
* Adding More Placeholders: Include a variety of placeholders such as `<verb>`, `<color>`, etc.
* Modifying the Script: Adjust the code to handle new types of placeholders or additional features.
## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (git checkout -b feature-branch).
3. Make your changes and commit (git commit -m 'Add feature').
4. Push to the branch (git push origin feature-branch).
5. Open a Pull Request.





## License

[MIT](https://choosealicense.com/licenses/mit/)

This project is licensed under the MIT License. See the `LICENSE` file for more details.
