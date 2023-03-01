# Sustainability-High-School-Mathematics

Project for the "HUM-433: How People Learn II" course at École polytechnique fédérale de Lausanne

## How to set up jupyter book

Check the installation guide on [this](https://jupyterbook.org/en/stable/start/overview.html) page (it's like any Python 
package).

## How to build a new version of the website

1. Go to the command line in this directory
2. Type "jupyter-book build book"
3. Check the output in the command line for any errors and run the output link in your browser

## How to push this build to GitHub?

1. In the "book" folder, copy the contents from the "html" folder into the "docs" (delete the old contents)
2. Make sure the "docs" folder contains the ".nojekyll" file. If not, create it!!!
3. Push your changes to GitHub. After a bit, the changes should become visible