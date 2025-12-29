# Spotify Analytics Dashboard
<p>
  This project is for end-to-end data processing and analysis of my personal Spotify streaming data for 2025. I am using Python to ingest and clean the JSON data,
  SQLite to transform and analyze the data, and Power BI to create an interactive and informative visualization dashboard.
</p>
<p>
  As a huge music enthusiast and stats nerd, I absolutely love Spotify Wrapped season. While it's always super interesting to see my year in review in terms of music, the broad overview has never felt fully satisfying, and I have always wanted to go deeper and really explore how my listening habits changed throughout the year. I felt like building my own analytics summary for the year seemed doable, and would be a fun way to practice my data analysis and visualization skills in Python, SQL, and Power BI while also being able to scratch the itch for truly in-depth streaming insights.
  The other slight issue I have with Wrapped is that the data collection ends early to mid-November, so I always feel like I'm not quite getting the entire picture. This project is reusable and adaptable to the entire year of data or any time period of interest. For now, the data runs from 01/01/2025-12/18/2025 since that is the date that I requested the streaming data JSON (though all that's really missing from the 18th until the time of writing is a bunch of Christmas music).
</p>
<h2>The Process</h2>
<h3>Data Cleaning</h3>
<p>
  The raw files include chronological entries for each stream containing various fields such as a timestamp, time played, and info about the track, artist, and stream. These raw files were ingested into a Jupyter Notebook, where Pandas was used to combine the files, filter out incomplete/non-song entries, and format/adjust series.
</p>
<h3>Data Transformation/Aggregation</h3>
<p>
  SQLite was used to convert and store the dataframe to a database due to its simplicity of integration with both Python and Power BI. In addition to storing the dataframe as a table, Multiple SQL views were created and stored in the database, containing larger/heavier data aggregations that would be used in the dashboard, such as streaming data by artist or by day.
</p>
<h3>Dashboard</h3>
<p>
  
</p>
