YouTube Data Analysis Streamlit Application


Overview


This Streamlit application is designed to facilitate access and analysis of data from multiple YouTube channels. Users can input a YouTube channel ID and retrieve relevant data such as channel name, subscribers, total video count, playlist ID, video ID, likes, dislikes, and comments for each video. The application provides options to store the data in a MongoDB database as a data lake, collect data for up to 10 different YouTube channels, and migrate selected channel data from the data lake to a SQL database. Additionally, users can search and retrieve data from the SQL database using various search options, including joining tables to get channel details.

Features


Retrieve YouTube Channel Data: Users can input a YouTube channel ID to retrieve relevant data including channel name, subscribers, total video count, playlist ID, video ID, likes, dislikes, and comments for each video.
Store Data in MongoDB: Option to store the retrieved data in a MongoDB database as a data lake.
Collect Data for Multiple Channels: Ability to collect data for up to 10 different YouTube channels and store them in the data lake with a single click.
Migrate Data to SQL Database: Users can select a channel name and migrate its data from the data lake to a SQL database as tables.
Query SQL Database: Ability to search and retrieve data from the SQL database using different search options, including joining tables to get channel details.
Data Visualization: Display the retrieved data in the Streamlit app using Streamlit's data visualization features such as charts and graphs.


Approach


Set up Streamlit App: Utilize Streamlit to build a user-friendly interface where users can interact with the application.
Connect to YouTube API: Use the Google API client library for Python to retrieve channel and video data from the YouTube API.
Store Data in MongoDB: Once data is retrieved from the YouTube API, store it in a MongoDB database as a data lake.
Migrate Data to SQL Database: After collecting data for multiple channels, migrate it to a SQL database such as MySQL or PostgreSQL.
Query SQL Database: Use SQL queries, possibly with a Python SQL library like SQLAlchemy, to retrieve and analyze data from the SQL database.
Display Data in Streamlit App: Present the retrieved data in the Streamlit app using Streamlit's data visualization features to enhance user understanding and analysis.


   

Technologies Used


Streamlit, 
Python, 
Google API client library, 
MongoDB, 
SQL Database (e.g., MySQL, PostgreSQL), 
SQLAlchemy (for interacting with SQL database), 
Docker (optional, for containerization)


Getting Started


Clone the project repository from GitHub.
Install the required dependencies using pip install -r requirements.txt.
Obtain API keys for accessing the YouTube API and configure them in the project.
Set up MongoDB and SQL database according to the provided schema.
Run the Streamlit app using streamlit run app.py.
Use the interface to input YouTube channel IDs, retrieve data, store in MongoDB, migrate to SQL, and query the database.



Acknowledgements


This project utilizes the YouTube API for data access.
We acknowledge the contributions of the open-source community for libraries and tools used in this project.


Feedback


We welcome feedback, suggestions, and contributions. Feel free to open an issue or submit a pull request on GitHub.

Feel free to modify and expand upon this README to suit the specific details and requirements of your Streamlit application for YouTube data analysis.
