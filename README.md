# Identifying wild mushrooms: what to forage, what to avoid? 

Through classification modeling, this project aims to classify mushrooms as edible or poisonous. 

In recent years, the popularity of mushrooms as a superfood and the understanding of their vast health benefits has surged.  What used to be typically seen as just a traditional food, mushrooms are now being widely consumed and acknowledged for their healing and health abilities.  With more and more people interested, foraging for mushrooms in the wild is likely to increase and I wanted to understand if edible/poisonous mushrooms could be easily indentified and what that looks like. 

## The Dataset 

The raw dataset utilized in this project was sourced from the UCI Machine Learning Repository. The dataset includes categorical characteristics on 8,124 mushroom samples from 23 species of gilled mushrooms. https://archive.ics.uci.edu/ml/datasets/Mushroom

- The target variable assessed was a class distinction of 'edible' or 'poisonous'. 
- The explanatory variables (originally 21) covered a range of descriptive and visual characteristics on the structure of each observed mushroom - such as, cap color, odor,ring number and stalk shape.

Target Distribution: 
![](/images/target.png)

## EDA 
- explored categorical features
- compared feature and class separation 

A few examples of categorical features within the dataset: 

![](/images/features.png)
![](/images/odor.png)
![](/images/spore.png)
![](/images/gillcolor.png)

## Conclusion & Takeaways

My tuned classification models all performed really well with the dataset. Logistic Regression, which had a score of 99% would normally be a great choice but given that the model predicted false negatives which could be deadly, and that the other tested models performed perfectly, the other models are much better suited to classify mushrooms.  Since my models performed so well, it was clear to me that they were able to identify specific traits that greatly influenced the classification of an edible versus poisonous mushroom. And that was exactly what I was hoping for!  

And finally, a few simple rules to identify a poisonous mushroom…

I was able to put together a simple list using what I learned from my feature importance analysis and EDA. That said, I am not an expert and this list should not be applied in the real world — but I was able to draw some conclusions which are worth sharing for the purpose of this project.

1. Odor: If the Mushroom has an odor, especially if the odor is not pleasant, it is likely to be poisonous.
2. Gill Size: If the gills are narrow, it is likely to be poisonous.
3. Spore Print Color: White, red, ‘chocolate’ are likely to be poisonous.
4. Bruises: If the mushroom does not have bruises, it is likely to be poisonous.
5. Stalk Surface Above Ring: If it appears silky, it is likely to be poisonous.



Contents of this project repository:

1. Data Folder: all csvs stored here and pkled data post cleaning
2. Notebooks Folder: all work in progress notebooks - cleaning, EDA, Modeling
3. Final.ipynb - final project notebook
4. Presentation - copy of final presentation deck
5. Images Folder: png files for graphs
