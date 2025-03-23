# YouTube API Client in Node.js

## Description
This is a Node.js client for interacting with the YouTube Data API. It allows users to fetch video details, search for videos, get channel information, and more.

## Features
- Search for YouTube videos
- Retrieve video details
- Fetch channel information
- List playlists and videos in a playlist
- Authentication with API Key or OAuth 2.0

## Prerequisites
- Node.js installed (v14 or later recommended)
- A YouTube Data API key or OAuth 2.0 credentials

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/youtube-api-client.git
   cd youtube-api-client
   ```
2. Install dependencies:
   ```sh
   npm install
   ```

## Configuration
1. Create a `.env` file in the root directory and add the following:
   ```env
   YOUTUBE_API_KEY=your_api_key_here
   ```
2. If using OAuth 2.0, configure your `client_secret.json` and set the path in the environment variables.

## Usage
Run the application:
```sh
node index.js
```

### Example API Calls
#### Search for Videos
```js
const { searchVideos } = require('./youtubeClient');
searchVideos('Node.js tutorial').then(console.log);
```

#### Get Video Details
```js
const { getVideoDetails } = require('./youtubeClient');
getVideoDetails('video_id').then(console.log);
```

## Dependencies
- `axios` - For making HTTP requests
- `dotenv` - For managing environment variables
- `googleapis` - Google API client for authentication (if using OAuth 2.0)

## Contributing
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License
This project is licensed under the MIT License.

## Contact
For any questions, feel free to reach out at [your-email@example.com].

