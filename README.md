# Transforming Web Behavior into Academic Program Personas
This project examined whether anonymous website behavior can be used to identify academic program personas among prospective students visiting Stockton University's website. Using Google Analytics data collected between March 28, 2026, and July 10, 2026, visitor interactions with academic program pages were analyzed using K-means clustering to uncover patterns of interest and engagement.

The analysis identified both broad and more detailed behavioral segments, including visitors focused on business, health professions, science, arts and humanities, and general exploration. While these patterns suggest that meaningful personas may exist within Stockton's website traffic, the clustering results showed relatively weak separation, indicating that the identified segments should be viewed as exploratory rather than definitive.

Although the findings do not currently support large-scale marketing or website personalization efforts, they demonstrate the feasibility of using behavioral analytics to develop audience personas from anonymous web traffic. Future work should focus on expanding the dataset and incorporating additional engagement metrics to improve the accuracy, stability, and practical value of persona-based segmentation.

## Environment
This project was developed in **Python** and is compatible with modern Python 3.x environments.

[Google Colab](https://colab.research.google.com/) provides a cloud-based Jupyter Notebook environment that allows users to run Python code directly in a web browser without requiring local installation or configuration. The [Anaconda Distribution](https://www.anaconda.com/platform/core) provides a preconfigured Python environment along with package and environment management tools that simplify dependency installation, project setup, and reproducibility across systems.

## Notebook Files
There are several Python notebook (.ipynb) files with this project.
- Practicum_Final_Run.ipynb - K-means model used in the Final Report
- data_exploration.ipynb - data exploration and cleanup of the Google Exploration
- google_exploration_connection.ipynb - script to connect with the Google Analyics API to request Exploration data. **This file is still in progress at this time**
- k_Means_Graduate_Only.ipynb - K-means model on just graduate degrees
- k_Means_Undergraduate_Only.ipynb - K-means model on just undergraduate degrees

## Data Collection
Data was obtained as a series of .csv files from Google Analytics Explorations collected on stockton.edu from March 28, 2026, through July 10, 2026. The analytics data from the CSV files were then imported, cleaned, explored, and analyzed using Python.
Dimensions used:
-	Page path and screen class - The page path from a website URL and screen class from a mobile application.
-	Landing page + query string - The page path and query string associated with the first pageview in a session.
-	Hour - The hour when a user activity occurred.
Metrics used:
-	Active users - The total number of active users.
-	Total users - The total number of unique users who have logged an event.
## Data Dictionary
| Variable        | Type        |	Description |
| --------------- | ----------- | ----------- |
| proxy_session_id | Object | Unique session identifier |
| page view variables | Integer | Counts of visits to individual program webpages during a session |
| unique_views | Integer | Number of distinct pages viewed in a session |
| just_url | Object | Base landing page extracted from proxy_session_id |

### Regulations to using the data
You are free to use my data in anyway you see fit, have fun.
