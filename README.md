# Tableau Project: EDA on the Distribution of Trees in Select Cities of the Bay Area
 Tableau Project: EDA on the Distribution of Trees in Select Cities of the Bay Area
# Tableau Project: EDA on the Distribution of Trees in Select Cities of the Bay Area
# INFO 247 Spring 2023

**Author:** Soorya Narayan Satheesh

## Table of Contents
1. [Initial Hypotheses or Questions](#initial-hypotheses-or-questions)
    1.1 [Motivation](#motivation)
    1.2 [Hypotheses](#hypotheses)
    1.3 [Analysis Plan](#analysis-plan)
2. [Data Source](#data-source)
    2.1 [Description](#description)
    2.2 [Source(s)](#sources)
    2.3 [Format](#format)
    2.4 [Transformations](#transformations)
3. [Exploration](#exploration)
    3.1 [Exploring Hypothesis 1: Uniform Distribution of Tree Species](#exploring-hypothesis-1-does-the-different-cities-of-the-bay-area-have-a-uniform-distribution-of-tree-species)
    3.2 [Exploring Hypothesis 2: Diversity in Tree Types](#exploring-hypothesis-2-is-there-diversity-in-the-tree-types-grown-in-the-bay-area)
    3.3 [Exploring Hypothesis 3: Variation in Average Tree Age](#exploring-hypothesis-3-is-there-variation-in-the-average-age-of-the-trees-in-the-bay-area)
    3.4 [Exploring Hypothesis 4: Relation Between Tree Number and Species Diversity](#exploring-hypothesis-4-is-there-any-relation-between-the-number-of-trees-in-a-street-and-the-diversity-of-species-there)
4. [Conclusion](#conclusion)
5. [References](#references)

---

## 1. Initial Hypotheses or Questions<a name="initial-hypotheses-or-questions"></a>

### 1.1 Motivation<a name="motivation"></a>
In the rapidly warming climate, urban areas are experiencing the negative impacts of climate change. Trees play a crucial role in mitigating these effects by improving aesthetics, reducing pollution, and supporting biodiversity. Understanding the distribution of trees in the urban cities of the Bay area, including their species and types, is essential for effective urban greening efforts and achieving climate change mitigation and biodiversity goals.

### 1.2 Hypotheses<a name="hypotheses"></a>
The following hypotheses were developed before and during the exploratory data analysis (EDA):
1. Do the different cities in the Bay area have a uniform distribution of tree species?
2. Is there diversity in the types of trees grown in the Bay area?
3. Is there variation in the average age of the trees in the Bay area?
4. Is there a relationship between the number of trees on a street and the diversity of species in that street?

### 1.3 Analysis Plan<a name="analysis-plan"></a>
The analysis plan includes the following steps:
1. Compile the datasets of seven Bay area cities using the "union" feature in Tableau.
2. Calculate the species-wise total number of trees in each city.
3. Group tree species into four major categories.
4. Analyze the variation in diameter at breast height (DBH) of the species across cities.
5. Analyze the streetwise variation in the number of trees.

---

## 2. Data Source<a name="data-source"></a>

### 2.1 Description<a name="description"></a>
The data used in this project is sourced from the "Raw urban street tree inventory data for 49 California cities" project by McPherson et al., funded by the US Government from 2006 to 2013. The project contains information on over 929,823 street trees in 49 Californian cities. For this EDA, the focus is on seven cities in the Bay area: Berkeley, Burlingame, Hayward, Palo Alto, Redwood City, San Mateo, and Walnut Creek. Additionally, an Excel file (citydata.xlsx) was created, providing information on the area, population (in 2020), and population density of each city using data from Wikipedia.

#### Table 1: Variables from Original Dataset Used in EDA
- `Idx`: Code of an individual tree for the city.
- `SpCode`: Short form of the tree species.
- `DBH`: Breast height diameter.
- `Street Name`: Name of the street in the city.
- `StreetNumber`: Number of the city street.
- `City`: Name of the city.
- `Botanical Name`: Botanical name of the tree species.
- `Common Name`: Common name of the tree.
- `Tree Type`: Special code that categorizes different tree species into one of twelve types.

#### Additional City Information (citydata.xlsx)
- `City`: Name of the city from the dataset.
- `Area_mi2`: Area of the city in square miles.
- `Population_2020`: Population of the city in 2020.
- `Population_Density`: Population density of the city.

### 2.2 Source(s)<a name="sources"></a>
- The main dataset is publicly available for download from the website of the US Forest Service: [Dataset Link](https://www.fs.usda.gov/rds/archive/catalog/RDS-2017-0010).
- Supplementary city information was collected from Wikipedia and compiled into an Excel file.

### 2.3 Format<a name="format"></a>
The main dataset was downloaded in CSV format, while the city information is stored in an XLSX file.

### 2.4 Transformations<a name="transformations"></a>
Key transformations performed:
- Combined the datasets of seven Bay area cities using the union feature in Tableau.
- Linked the tree inventory datasets with the Excel file containing city information.
- Grouped tree types into four major categories: Broadleaved Deciduous, Broadleaved Evergreen, Conifer Evergreen, Palm Evergreen, and Others.

---

## 3. Exploration<a name="exploration"></a>

### 3.1 Exploring Hypothesis 1: Uniform Distribution of Tree Species<a name="exploring-hypothesis-1-does-the-different-cities-of-the-bay-area-have-a-uniform-distribution-of-tree-species"></a>
- Analyzed the number of trees and tree species in different cities.
- Investigated the relationship between species diversity and city population and population density.
![Figure 1-Tree numbers analysis](../Tableau-Project--EDA-on-the-Distribution-of-Trees-in-Select-Cities-of-the-Bay-Area/935844828/Image_001.gif)

### 3.2 Exploring Hypothesis 2: Diversity in Tree Types<a name="exploring-hypothesis-2-is-there-diversity-in-the-tree-types-grown-in-the-bay-area"></a>
- Explored the distribution of tree types (Broadleaved Deciduous, Broadleaved Evergreen, Conifer Evergreen, Palm Evergreen, and Others) in different cities.
![Figure 2-Tree type distribution](../Tableau-Project--EDA-on-the-Distribution-of-Trees-in-Select-Cities-of-the-Bay-Area/935844828/Image_003.gif)

### 3.3 Exploring Hypothesis 3: Variation in Average Age of Trees<a name="exploring-hypothesis-3-is-there-variation-in-the-average-age-of-the-trees-in-the-bay-area"></a>
- Analyzed the distribution of the diameter at breast height (DBH) of trees by city and type.
![Figure 3-Tree DBH distribution](../Tableau-Project--EDA-on-the-Distribution-of-Trees-in-Select-Cities-of-the-Bay-Area/935844828/Image_004.gif)

### 3.4 Exploring Hypothesis 4: Relation Between Tree Number and Species Diversity<a name="exploring-hypothesis-4-is-there-any-relation-between-the-number-of-trees-in-a-street-and-the-diversity-of-species-therea"></a>
- Analyzed the street wise number of trees across the seven cities.
![Figure 3-Tree DBH distribution](../Tableau-Project--EDA-on-the-Distribution-of-Trees-in-Select-Cities-of-the-Bay-Area/935844828/Image_005.gif)

## 4 	CONCLUSION <a name="conclusion"></a>

This EDA project helped me understand the nitty-gritties of selection of dataset and working with a wide variety of visualization. This project helped changed several presumptions I had about the nature of trees and environment in the Bay area. When we talk of trees, we think of forests in the Yosemite but we forget that the urban trees also play a crucial role in helping the environment as well as the humans living near them. Thus using the insights gleaned from this analysis the city planners could plan ahead to increase the diversity of tree species in the cities to help increase urban biodiversity.


## 5	REFERENCES <a name="references"></a>

McPherson, E. Gregory; van Doorn, Natalie S.; de Goede, John. 2017. Raw urban street tree inventory data for 49 California cities. Fort Collins, CO: Forest Service Research Data Archive. https://doi.org/10.2737/RDS-2017-0010

Wikimedia Foundation. (2023, February 23). Berkeley, California. Wikipedia. Retrieved March 8, 2023, from https://en.wikipedia.org/wiki/Berkeley,_California

Wikimedia Foundation. (2023, February 23). Redwood City, California. Wikipedia. Retrieved March 8, 2023, from https://en.wikipedia.org/wiki/ Redwood_City,_California

Wikimedia Foundation. (2023, February 23). Burlingame, California. Wikipedia. Retrieved March 8, 2023, from https://en.wikipedia.org/wiki/ Burlingame,_California

Wikimedia Foundation. (2023, February 23). Walnut Creek, California. Wikipedia. Retrieved March 8, 2023, from https://en.wikipedia.org/wiki/ Walnut_Creek,_California

Wikimedia Foundation. (2023, February 23). Palo Alto, California. Wikipedia. Retrieved March 8, 2023, from https://en.wikipedia.org/wiki/ Palo_Alto,_California

Wikimedia Foundation. (2023, February 23). Hayward, California. Wikipedia. Retrieved March 8, 2023, from https://en.wikipedia.org/wiki/ Hayward,_California

Wikimedia Foundation. (2023, February 23). San Mateo, California. Wikipedia. Retrieved March 8, 2023, from https://en.wikipedia.org/wiki/ San_Mateo,_California