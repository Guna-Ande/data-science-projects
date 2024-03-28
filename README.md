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
Example Data Extraction from YouTube to MongoDB
json

{
  "Channel_Name": {
    "Channel_Name": "Example Channel",
    "Channel_Id": "UC1234567890",
    "Subscription_Count": 10000,
    "Channel_Views": 1000000,
    "Channel_Description": "This is an example channel.",
    "Playlist_Id": "PL1234567890"
  },
  "Video_Id_1": {
    "Video_Id": "V1234567890",
    "Video_Name": "Example Video 1",
    "Video_Description": "This is an example video.",
    "Tags": ["example", "video"],
    "PublishedAt": "2022-01-01T00:00:00Z",
    "View_Count": 1000,
    "Like_Count": 100,
    "Dislike_Count": 10,
    "Favorite_Count": 5,
    "Comment_Count": 20,
    "Duration": "00:05:00",
    "Thumbnail": "https://example.com/thumbnail.jpg",
    "Caption_Status": "Available",
    "Comments": {
      "Comment_Id_1": {
        "Comment_Id": "C1234567890",
        "Comment_Text": "This is a comment.",
        "Comment_Author": "Example User",
        "Comment_PublishedAt": "2022-01-01T00:01:00Z"
      },
      "Comment_Id_2": {
        "Comment_Id": "C2345678901",
        "Comment_Text": "This is another comment.",
        "Comment_Author": "Another User",
        "Comment_PublishedAt": "2022-01-01T00:02:00Z"
      }
    }
  },
  "Video_Id_2": {
    "Video_Id": "V2345678901",
    "Video_Name": "Example Video 2",
    "Video_Description": "This is another example video.",
    "Tags": ["example", "video"],
    "PublishedAt": "2022-01-02T00:00:00Z",
    "View_Count": 2000,
    "Like_Count": 200,
    "Dislike_Count": 20,
    "Favorite_Count": 10,
    "Comment_Count": 30,
    "Duration": "00:10:00",
    "Thumbnail": "https://example.com/thumbnail.jpg",
    "Caption_Status": "Not Available",
    "Comments": {}
  }
}
Example SQL Tables
Table structure to be added based on your SQL database schema.

Technologies Used
Streamlit
Python
Google API client library
MongoDB
SQL Database (e.g., MySQL, PostgreSQL)
SQLAlchemy (for interacting with SQL database)
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
