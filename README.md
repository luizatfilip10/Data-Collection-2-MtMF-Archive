# Preservation and Analysis of the Movies that Matter Festival Film Archive 

<img src="https://moviesthatmatter.nl/content/uploads/2021/01/MTM_mainlogo_All_web.png">

## How are human rights themes distributed and represented across languages, countries, and time in the Movies that Matter Festival Film Archive?

This project serves both a preservation and a research purpose. From a preservation perspective, we will scrape all 1,202 film pages, including their metadata, from the <a href="https://moviesthatmatter.nl/en/festival/archive/film-archive/#/" target="_blank">Movies that Matter Film Archive</a>, which, to our knowledge, has not been done before. This dataset is rich for preservation purposes, not only because it covers screened films from 2009 to 2026, but the diversity of themes, regions, and years ensures that the Movies that Matter Film Archive captures a comprehensive historical record of human rights–focused cinema, preserving both the films themselves and the festival’s curatorial decisions for future access and study. Although the Movies that Matter Festival Archive also includes pages about the artists and activists who participate in the festival, we do not include this data in our project, as doing so would change our research aim.

From a research perspective, we will use this dataset to conduct computational research based on information from individual film pages. This includes assigned themes, relevant countries, MtMF year, title, film description, director, producer, release year, country of production, duration, spoken languages, subtitle language, production company, and world sales. The goal of this project is to analyze and visualize global human rights issues as represented through the film archive’s thematic classifications. This is significant because it reveals how curated film archives shape the visibility, framing, and geographic distribution of human rights issues, highlighting which themes are emphasized and which may be underrepresented. This analysis could also offer viewers a clear overview of global human rights concerns as represented in the film archive, potentially serving as a resource for the festival’s website.

##  :movie_camera: Structure
This repository contains various files, these include:
|  Title | Type | Content|   
| ----- | --- | --- |
| Preservation | `.ipynb` | Jupyter Notebook containing the code for scraping and creating the data frame, includes an active learning exercise and ends with saving the csv file. |
| Analysis | `.ipynb` | Jupyter Notebook containing code in which we used the generated content from the preservation notebook, in order to analyze and visualize the data and ends with critical thinking exercise. |
| Report | `.ipynb` | Jupyter Notebook containing the report of the whole process. |
| df_mtmf | `.csv` | File containing the entire scraped corpus. |
| Images | `.png`, `.jpg` | Directory containing all the images used. |


## :video_camera: CSV key 
We have the following columns in order:
| Name | Type |
| --- | --- | 
| movie_url | link to each movie |
| title | string |
| description | string |
| themes | list of strings |
| relevant_countries | list of strings |
| mtmf_years | numerical |
| director | list of strings |
| producer | list of strings |
| year_release | numerical |
| country_of_production | list of strings |
| duration | numerical |
| spoken_language | list of strings |
| subtitles | list of strings |
| production_company | list of strings |
| world_sales | list of strings |

Note: We saved most of the columns as a list of strings because some movies contain multiple directors/producers/themes etc, therefore it is important to have them separated in order to create visualizations and make the analysis.

## :computer: How to use and what you need
You will need software that can run Jupyter Notebook (`.ipynb`) files in order to access this repository. For the code to function correctly, you must additionally make sure that the necessary Python modules and libraries are installed:
- pandas
- requests
- BeautifulSoup
- time
- selenium
- re
- plotly.express
- plotly.io
- matplotlib.pyplot
- matplotlib

## :clapper: Intended use 
Beyond the scope of this project, the df_mtmf dataset could serve as a valuable resource for other researchers. It could be used to compare thematic patterns across multiple film festivals, investigate regional trends in human rights representation, or explore the relationship between curatorial decisions and audience engagement. Additionally, computational approaches could be applied to model how certain themes are selected, track changes in human rights discourse over time, or analyze the network of films, countries, and topics to uncover broader patterns in global human rights cinema.

## :camera: Licenses 
All data collection is conducted for educational purposes only. Because the website does not provide a robots.txt file, the code and collected data are stored in a private GitHub repository with access restricted to the professors supervising the project, ensuring responsible and ethical data handling.


## :bust_in_silhouette: Collaborators

This repository was created by Andreea-Gabriela Ion, Minja Cvetkovski and Luiza Teodora Filip

- https://github.com/aandreeaion &rarr; Preservation notebook and part of Analysis notebook

- https://github.com/Minja-Cvetkovski &rarr; part of Report notebook, part of Analysis notebook and part of README file

- https://github.com/luizatfilip10 &rarr; part of Report notebook, part of Analysis notebook and part of README file

<b> Note: We proofread everything and we verified eachothers sections </b>








