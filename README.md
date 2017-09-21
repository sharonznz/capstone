# capstone
Capstone project for Udacity Machine Learning Engineer Degree

Files: 

download_as_text_files.ipynb: Scrapes press releases from political party websites and saves in working directory (You may need to manually create 6 subdirectories called act green national nzfirst maori labour respectively). The releases are always being updated (the election is this weekend), so the file will not give exactly the dataset I used, but there should be a large degree of crossover if run relatively soon.

Preprocess_fit.ipynb: Reads in the resulting text files and preprocesses them ready for Scikit-learn. Fits and then optimises a Naive Bayes model.

Vet_optimised_model.ipynb: Re-fits the optimised Naive Bayes and performs various robustness checks. Fits a SVC classifier. Tests the model on newly downloaded more recent data releases (see last file described below)

download_latest_as_test_set.ipynb: An adapted version of the earlier download file that loads down the most recent releases and saves them in a "test" subfolder. Checks for and deletes any crossover with the original dataset.

Python packages: None are particularly obscure. BeautifulSoup was used for webscraping. Scikit-learn was used for model estimation. All import statements are at the top of the notebooks.
