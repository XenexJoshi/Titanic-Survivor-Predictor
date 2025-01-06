Titanic Survivor Predictor:

This program contains a machine-learning model that attempts to learn and predict whether an individual onboard the Titanic survived based on their demographic information including their age, assigned sex at birth, class on the ship, and the boarding location where the individuals boarded the Titanic. The dataset was obtained by web-scraping from https://titanicfacts.net/, using requests and BeautifulSoup to extract the respective tables corresponding to the survivors and the victims. The extracted datasets were processed using the pandas data frame, which includes identifying the individual's assigned sex based on the salutation prefixed to their first name. The raw web-scraped data can be found in the data/ directory. 

The next part of the project involves combining the two datasets corresponding to the survivors' and victims' datasets to compile a single .csv file containing the demographic information and the survival status of all passengers on the Titanic. The data is preprocessed by converting string data types into tokens(int and float) to allow running different machine learning algorithms. The project involves a decision tree algorithm, which is then boosted using an ensemble method i.e. the random forest algorithm, naive-bayes algorithm, and an SVM, which is fine-tuned using cross-validation. Finally, the program uses a neural network to train and predict the survival of passengers on the Titanic. After implementing all these methods, we obtain a prediction accuracy of 79.2% on the testing set.

The program also contains a fun predictor function based on the learned models that predict whether an individual in the modern age would have survived the Titanic based on the demographic information that they pass as arguments to the function. This is meant to be a fun aspect of the project, has some randomized components, and is meant to be recreational, not meant to be taken seriously.

Required modules:

    pandas
    numpy
    tensorflow
    matplotlib
    sklearn

To run the .ipynb file, install the above-mentioned modules after navigating to the file after cloning the repository, and run the .pynb file.

Relevant links and references:

https://titanicfacts.net/

https://www.cruisemummy.co.uk/titanic-ticket-prices/
