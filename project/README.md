# Title
**World 2017: Total War**

# Abstract
Seemingly whimsical, the title of this project encloses the harsh reality of how astoundingly primitive we are in the 21st century and how little has actually changed since Medieval times. We attempt to modernise our society in many aspects, invent new technology to make everyday life more pleasant, but at the end of the day, we witness so much violence, intolerance and hatred. Independent of the fact whether it is an inter-country conflict for territory, an organisation requesting rights, a state or region fighting for independence, the truth is these clashes result in numerous casualties, direct or collateral, ruined societies, destroyed lives and terrible loss. And there are much more sparkles on the edge of kindling a fire.

The goal of this project is to make an attempt at uncovering the shocking reality about world conflicts that few people know about because it may not be or have been in the spotlight. Hopefully, observing the aggregated information visualised in a nicely presentable way will help raise awareness of what has been happening in recent history or at the present moment, and bring incentive to start building an improved version of the World.

# Research questions

* Aggregate the data for each country and make a country profile of all the conflicts available in the dataset
	* list of events the country was involved in
	* number of casualties per conflict and per year
	* analysis of the intensity of conflicts
* Aggregate the data on a regional basis
	* analysis of the intensity of conflicts
* Identify relevant different entities which are not countries (organizations) and create a profile
	* list of events the country was involved in
	* number of casualties per conflict and per year
* Establish a conflict graph showing the actors and their interactions through engagement in conflict episodes
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
* UCDP/PRIO Armed Conflict Dataset version 17.1
* UCDP Battle-Related Deaths Dataset

Additional datasets to enrich the information provided by the formerly mentioned:
* UCDP Monadic Conflict Onset and Incidence Dataset

Metadata and helper datasets:
* UCDP Actor List
* Gleditsch and Ward list of independent countries

# A list of internal milestones up until project milestone 2

1. Carefully read the provided codebooks for each of the primary datasets -> *done*
	* understand the jargon and the technical terms contained in the attribute names or values -> *done*
2. Analyse the primary datasets, especially the categorical attributes whose values are explained in the codebook -> *done*
3. Isolate a subset of project-relevant features from each dataset -> *done*

# Overview of the work done for milestone 2

It is worth noticing that even though they are "real-world" datasets, the UCDP datasets lack the disorder, chaoticity and general "messiness" that other datasets usually encompass. This is understandable if we look into the background, into the data collection process which was done by professionals in a systematic manner, researchers who used well-precised methodologies and invested a non-negligible amount of work into the correctness and completeness of the provided data. Therefore, quite honestly, much of the standard preprocessing steps were unnecessary as they were either already applied or simply those issues were nonexistant.

For every dataset we explored whether any of the features of interest contained any missing values. Everything else boiled down to the analysis of the dataset size, the type of the variables, the ranges of the variables where we judged useful to have that information and the number of unique observed events.

As the data is rather small in its volume, quite comprehensible without the need of significant computational power, surprisingly clean and consistent, and very well documented and described, the biggest challenge was to get familiar with the terminology and the meaning of the features that are used to describe the data. After extensive reading of the so-called "codebooks" that accompany every dataset, we put together tables explaining the used variables accross the different datasets, stating the name, the type and a detailed meaning, as this is crucial to understand how and why some steps are made or some decisions are taken. Furthermore, we give definition of some of the jargon that is used throughout the project. For each dataset we also briefly discuss the necessity of it and the reasons it was chosen in terms of the intentions we have for the next milestone.

As stated in the abstract itself, the purpose of this project is to aggregate and analyse the data, draw conclusions and use different visualisation techniques in order to present them in a way that will make it very easy for the reader to understand the point. We will not dive into supervised or unsupervised learning techniques, but rather employ data visualisation such as graphs, network diagrams, maps and other plots to discover the relationships between the conflict actors, to collect and display all the information contained in the different datasets in one place.

# Planned activities for project milestone 3

1. Choropleth maps with interactive features showing the number of conflicts on a particular location and the number of battle-related deaths
2. Interactive map with markers pinpointing the geographical locations where there was an armed conflict episode in the period 1989-2016
3. Network diagram visualising a graph structure of interconnected nodes which represent conflicted sides
4. Integration of all data, plot statistics in one interactive platform

Note: In order to win in interactivity we are considering using Leaflet directly, as a framework, but this will require tweaking the code. Leaflet provides more interactivity, but will cost us some flexibility in data manipulation, as it used with JavaScript and not Python. This is the reason why we didn't proceed to building the final version of the maps as we still want to take some time to weigh the pros and cons of this visualization choice.
