# Song Recommendation Engine

This project is a song recommendation engine that utilizes the Spotify API and the K-nearest neighbors algorithm (KNN) to recommend similar songs based on the user's top tracks.

## Features

- Fetches the user's top tracks from their Spotify account.
- Extracts audio features of the user's top tracks using the Spotify API.
- Trains a KNN model using the extracted audio features.
- Fetches a song catalog playlist from Spotify.
- Calculates the similarity between the user's top tracks and songs in the catalog using the KNN model.
- Ranks and displays the top recommended songs.

## Setup

1. Create a Spotify Developer account and set up a new application to obtain the required client ID and client secret.
2. Update the `client_id` and `client_secret` variables in the code with your own credentials.
3. Install the required Python packages by running `pip install -r requirements.txt`.
4. Run the script and follow the authentication prompts to grant access to the Spotify API.

## Usage

1. Run the script using `python song_recommendation_engine.py`.
2. The script will retrieve your top tracks and calculate the most similar songs from the provided catalog playlist.
3. The top recommended songs will be displayed in the console.

## Customize

- You can modify the `limit` parameter when fetching the user's top tracks to specify the number of tracks to consider.
- Adjust the `n_neighbors` parameter when training the KNN model to change the number of similar songs recommended.
- Update the `playlist_id` variable to target a different Spotify playlist for the song catalog.

## License

This project is licensed under the [MIT License](LICENSE).
