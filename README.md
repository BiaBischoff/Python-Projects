# Python-Projects
Collection of some silly Python projects:
1-) generate a band name
2-) Encode/Decode
3-) Calculates tip amount
4-) Returns the index of the numbers in the list that sum up to the target variable
5-) Music Genre Classification with PCA (more details below)

**CASE DESCRIPTION:**

![Blue And Red Modern Music Youtube Thumbnail](https://github.com/BiaBischoff/Python-Projects/assets/104466669/dd740784-8f75-4a10-951f-6953de424138)

**Objective**

In the era of digital streaming, there’s an increasing need to categorize and recommend music based on genres. By analyzing various musical features extracted from tracks, we can delve deeper into their defining patterns. In this music genre classification project, you’ll work with a dataset containing various musical features extracted from tracks across different styles.

Please note that while this music genre classification dataset is extensive, it is incomplete. A significant portion of the records lacks specific genre information.

Your primary task is to predict the genres of these unlabeled tracks.

To accomplish this, you’ll employ Principal Component Analysis (PCA) to reduce the dimensionality of the dataset. By transforming the abundant features into principal components, you’ll streamline the data, making it more manageable and revealing patterns that are not immediately obvious in the raw data. The principal components you’ve derived will form the foundation for the next step in the project—employing a supervised machine learning algorithm, with a focus on the well-known logistic regression technique.

Why Principal Component Analysis (PCA)?

Music tracks are complex entities with numerous inherent features. Some of these features might be correlated. For instance, specific rhythm patterns might be prevalent in rock and blues. In this machine learning project, PCA can assist in reducing redundancy by transforming correlated musical features into a set of linearly uncorrelated variables or principal components. Reducing dimensionality can drastically improve the performance of classification algorithms by eliminating noise.

The features in the music genre classification dataset are designed to be intuitive and accessible allowing you to focus on the core concepts of PCA and machine learning without the need for specialized audio knowledge.

Prepare to dive deep into the layers of musical data and discover the patterns that help outline the musical genres.

**FINDINGS:**

Dataset distribution:

![image](https://github.com/BiaBischoff/Python-Projects/assets/104466669/a485f92d-04a6-46cd-ad26-1844513ef36b)

After removing null data from the dataset, we can check the correlations:

![image](https://github.com/BiaBischoff/Python-Projects/assets/104466669/474824cd-02ce-45a5-9a9a-2fcd4eac89b4)

We standardize the data for PCA analysis and calculate the number of total components: 12 components

But the project instructed to get the number of components that explained 80% of variance: 8 components

![image](https://github.com/BiaBischoff/Python-Projects/assets/104466669/08379b1d-88cd-4e41-9bb9-a48b3c43a2e7)

We then split the data and apply logistic regression to predict some missing genres. 

![performance](https://github.com/BiaBischoff/Python-Projects/assets/104466669/395be3be-6b08-4ba9-bd93-644501b656dd)

For all originally missing genre rows, we now have a new value predicted by our algorithm:

![predicted](https://github.com/BiaBischoff/Python-Projects/assets/104466669/c9e781a1-a5e7-4282-a3ba-93f1d13b998f)

