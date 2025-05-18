# Spotify-Music-Analysis-Dashboard-Built-by-Oladipupo-John
# This project is an interactive Power BI dashboard that visualizes and analyzes streaming patterns and song features from a Spotify dataset. The report provides insights into music consumption trends across time, months, and weekdays while highlighting track-level attributes such as danceability, energy, and popularity.

# Project Overview
# This dashboard was created to explore and present insights from a Spotify dataset comprising 952 tracks with data on streams, release dates, track details, audio features, and artist popularity. The project aims to highlight:
# Trends in music streaming over time
# Monthly and daily streaming behavior
# Characteristics of top streamed tracks
# Track-level audio attributes like energy, danceability, and speechiness
# Listener behavior patterns and artist performance
# Project Overview
# This dashboard was created to explore and present insights from a Spotify dataset comprising 952 tracks with data on streams, release dates, track details, audio features, and artist popularity. The project aims to highlight:
# Trends in music streaming over time
# Monthly and daily streaming behavior
# Characteristics of top streamed tracks
# Track-level audio attributes like energy, danceability, and speechiness
# Listener behavior patterns and artist performance

# 📌 Objectives
# Identify the most streamed songs and artists

# Analyze streaming behavior by month and day

# Visualize streaming trends based on release dates

# Break down audio features like danceability, energy, and speechiness

# Provide an interactive and dynamic experience for exploring Spotify data
# 🛠 Tools Used
# Power BI	Data modeling, dashboard creation, visualization
# DAX	Measures, calculated columns, date intelligence
# Excel	Initial data formatting and preparation
# 📈 Key Visuals in the Dashboard
# 🟢 Header KPIs
# Total Streams: 489 billion
# No of Tracks: 952
# Average Streams per Track: 514 million
# 📉 Streaming Trends by Release Date
# A line graph showing how streaming volume changed over time, from the 1940s to 2020s
# Peaks identify era-defining tracks or surges in streaming activity

# 📅 Monthly Streaming and Track Trends
# A matrix-style table showing:
# Number of tracks released in each month
# Average streams per track for each month
# Useful to identify which months yield the most popular or abundant music

# 📆 Daily Streams
# Bar chart breaking down:
# Stream volumes by day of the week
# Identifies Fridays as the peak streaming day (often due to new music releases)

# 🌟 Artist Most Streamed Track
# Highlighted card showing Blinding Lights by The Weeknd Includes:
# Track Key
# Launch Date
# Scale Type
# Total Plays
# Audio features: Danceability %, Speechiness %, Energy %
# 🎵 Top 6 Most Streamed Tracks
# Visual gallery of the top 6 songs, showcasing:
# Track cover image
# Artist name
# Relative popularity based on stream counts
# 📊 Measures Created in DAX
# Total Streams = SUM('Spotify Dataset'[Streams])

# Average Streams = AVERAGE('Spotify Dataset'[Streams])

# No of Tracks = COUNT('Spotify Dataset'[Track Name])

# Top Streamed Song = CALCULATE(MAX('Spotify Dataset'[Streams]))

# Monthly Streams = SUMX(SUMMARIZE('Spotify Dataset', 'Spotify Dataset'[Month], "MonthlySum", SUM('Spotify Dataset'[Streams])), [MonthlySum])

# Daily Streams = SUMMARIZE('Spotify Dataset', 'Spotify Dataset'[Day], "TotalStreams", SUM('Spotify Dataset'[Streams]))

# (Additional DAX measures can be listed here based on what's in your actual PBIX.)

### ✅ Recommendations
# 1. **Release on Fridays**: Most streams occur on Fridays — align track drops accordingly.  
# 2. **Focus on Danceable, High-Energy Songs**: These attributes correlate with streaming success.  
# 3. **Target High-Performing Months**: January and September show strong average stream performance.  
# 4. **Boost Promotions Around Top Tracks**: Leverage streaming stars for audience engagement.  
# 5. **Curate Audio Feature-Specific Playlists**: Use characteristics like speechiness or energy for smart playlisting.

