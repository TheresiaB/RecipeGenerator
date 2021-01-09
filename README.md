### About the Project
This recipe generator was developed by a team of 7 students as part of the course "Business Process Innovation Lab" from the M.Sc. in Business Intelligence and Process Management. The application takes a list of ingredients as input, selects those that go well together, and returns suitable preparation modes for each of them. The presented result evolved within a period of 6 weeks. This project was inspired by the food2vec repository  https://github.com/altosaar/food2vec and is based on recipes from allrecipes.com derived via https://eightportions.com/datasets/Recipes/
A generated recipe was tested in real life and could by enjoyed after using some creativity in the preparation phase. The ingredient selection can be an inspiration on what to combine. Happy testing and enjoy!

### Prerequisites
You must have pandas, numpy, gensim.models and sklearn.cluster and Flask (for API) installed.

Flask version: 0.12.2
conda install flask=0.12.2  (or) pip install Flask==0.12.2

### Project Structure
This project has three major parts :
1. app.py - This is the main file where the recipe generation happens. It loads the pickle-files as well as the input ingredients and returns the generated recipe. It holds the two main defined functions where firstly, the input ingredients are scanned and those that go well together are returned, and secondly, for each returned input ingredient a preparation mode is defined. 
2. template - This folder contains the HTML template (index.html) which allows the user to enter ingredients and displays the outcome recipe.
3. static - This folder contains the css folder with style.css file which has the styling required for our index.html file as well as the image displayed on the webpage. 

### Running the project

1. Run app.py using below command to start Flask API. Ensure that you are in the project home directory. 
```
python app.py
```
By default, flask will run on port 5000.

2. Navigate to URL http://127.0.0.1:5000/ (or) http://localhost:5000

You should be able to view the homepage.

Enter some ingredients only separated by spaces and hit the "Generate Recipe"-Button 

If everything goes well, you should  be able to see the generated recipe as single steps on the HTML page!
check the output here: http://127.0.0.1:5000/predict

