# Frappe Technical Docs

## Installation and Development

- Mkdocs is a python library for creating documentations using _Markdown_ language
- To use Mkdocs first we need to create a python environment.

  ```sh
  # linux and mac
  python3 -m venv venv --prompt "mkdocs"

  # windows
  py -m venv venv --prompt "mkdocs"
  ```

- Then Activate the newly created environment using the following command

  ```sh
  # linux and mac
  source venv/bin/activate

  # windows
  .\venv\Scripts\activate
  ```

- Install the requirements using the following command

  ```sh
  pip install -r requirements.txt
  ```

- The `requirements.txt` file contains material-mkdocs which is a theme used with Mkdocs.

- To run the server use the following command

  ```sh
  mkdocs serve
  ```
