# AnimeRecommendation

## Setting Up the Environment

Follow the steps below to set up your local development environment:

1. **Create a Virtual Environment**

   Use the following command to create a new virtual environment named `.venv`:

   ```bash
   python -m venv .venv
   # or for specific Python version
   python3.9 -m venv .venv
   ```

2. **Activate the Virtual Environment**

   Depending on your shell, use one of the following commands to activate the virtual environment:

   On Windows (Command Prompt):

   ```bash
   .venv\Scripts\activate
   ```

   On Windows (Git Bash):

   ```bash
   source .venv/Scripts/activate
   ```

3. **Install Required Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

To deactivate the virtual environment when you're done, use:

```bash
deactivate
```

If you install additional libraries and want to save them as dependencies, use:

```bash
pip freeze > requirements.txt
```

## Selecting the Virtual Environment in VS Code

After setting up and activating the virtual environment, you need to select it as your interpreter in VS Code. Follow these steps:

1. Open the Command Palette (`Ctrl+Shift+P`).
2. Type and select `Python: Select Interpreter`.
3. In the dropdown, choose the interpreter that corresponds to the `.venv` virtual environment you created.

Now, VS Code will use the Python interpreter in the virtual environment for running Python scripts and debugging.

## Dataset

We are using the Anime Recommendations Database from Kaggle. Follow the steps below to download and set up the dataset:

1. Visit the [Anime Recommendations Database](https://www.kaggle.com/CooperUnion/anime-recommendations-database) on Kaggle.

2. Click on the "Download (5 MB)" button on the right side of the screen. This will download a zip file named `anime-recommendations-database.zip`.

3. Extract the `anime.csv` and `rating.csv` files from the downloaded zip file.

4. Create a `data` folder in the root directory of your project if it doesn't exist already.

5. Move the `anime.csv` and `rating.csv` files into the `data` folder.

Your directory structure should now look like this:

```bash
root
│   README.md
│   ...
│
└───data
│   │   anime.csv
│   │   rating.csv
│
└───.venv
    │   ...
```
