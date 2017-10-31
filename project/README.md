# Title
**World 2017: Total War**

# Abstract
Seemingly whimsical, the title of this project encloses the harsh reality of how astoundingly primitive we are in the 21st century and how little has actually changed since Medieval times. We attempt to modernise our society in many aspects, invent new technology to make everyday life more pleasant, but at the end of the day, we witness so much violence, intolerance and hatred. Independent of the fact whether it is an inter-country conflict for territory, an organisation requesting rights, a state or region fighting for independence, the truth is these clashes result in numerous casualties, direct or collateral, ruined societies, destroyed lives and terrible loss. And there are much more sparkles on the edge of kindling a fire.

The goal of this project is to make an attempt at uncovering the shocking reality about world conflicts that few people know about because it may not be or have been in the spotlight. Hopefully, observing the aggregated information visualised in a nicely presentable way will help raise awareness of what has been happening in recent history or at the present moment, and bring incentive to start building an improved version of the World.

# Research questions

* Aggregate the data for each country and make a country profile of all the conflicts available in the dataset
	* list of events the country was involved in
	* number of casualties aggregated in a comprehensible manner
* Identify relevant different entities which are not countries (organizations) and create a profile
	* list of events the country was involved in
	* number of casualties aggregated in a comprehensible manner
* Establish a conflict graph showing the actors or regions and their interactions
* Identify "problematic" regions on the World map with recent or on-going conflicts
* Rate regions by safety based on the history of conflicts they were involved in and their respective magnitude
	* number of conflicts
	* time since last conflict
	* number of casualties
	* gravity of the conflicts

# Dataset

For the purpose of the reasearch project, the team will be using the UCDP datasets provided for download on the website: http://ucdp.uu.se/downloads/.

The primary datasets of interest are:
* UCDP Georeferenced Event Dataset (GED) Global version 17.1 (2016)
* UCDP Dyadic Dataset version 17.1
* UCDP One-sided Violence Dataset
* UCDP Battle-Related Deaths Dataset

Datasets to enrich the information provided by the formerly mentioned:
* UCDP Conflict Termination Dataset version 2-2015

Datasets to provide metadata or facilitate the merge of other datasets:
* ID translation tables
* UCDP Actor List

Preliminary inspection of the format and the data itself shows that the datasets were built in a systematic manner, with a significant amount of care taken to the completeness of data - missing values do not indicate error in measurement, but the data is truly inexistant. Furthermore, a separate codebook providing term definitions and attribute explanations is available per dataset. This already provides significant help in the process of exploratory data analysis and pre-processing, because the semantic, the attribute type, ranges and potential issues are discussed in the codebook.

The volume of the data is quite comprehensible, since the datasets contain around a dozen attributes and in the order of 100K samples.

# A list of internal milestones up until project milestone 2

1. Carefully read the provided codebooks for each of the primary datasets
	* understand the jargon and the technical terms contained in the attribute names or values
2. Analyse the primary datasets, especially the categorical attributes whose values are explained in the codebook
3. Isolate a subset of project-relevant features from each dataset

# Questions for TAa

