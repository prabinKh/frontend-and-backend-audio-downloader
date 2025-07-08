
# YouTube Audio Downloader

## Overview

The YouTube Audio Downloader is a Django-based application that allows users to manage YouTube channels, download audio files, and create personalized playlists. It utilizes background tasks to download and update media content regularly and offers both a web interface and an API for accessing the media files.

## Features

- **Channel Management**: Users can add and manage YouTube channels.
- **Media Download**: Audio files can be downloaded from YouTube videos directly.
- **Playlist Creation**: Create and manage playlists of your favorite songs.
- **Liked Songs & Downloads**: Mark songs as liked and manage your downloads.
- **Background Tasks**: Automatic fetching and downloading of media using `yt-dlp`.
- **API Access**: Access to media information through API endpoints.

## API Endpoints

- `/api/audio/`: List audio files.
- `/api/playlists/create/`: Create a new user playlist.
- `/api/playlists/`: List user playlists.
- `/api/liked-songs/create/`: Like a song.
- `/api/liked-songs/`: List liked songs.
- `/api/downloaded-songs/create/`: Add song to downloads.
- `/api/downloaded-songs/`: List downloaded songs.
- `/api/channelid/<str:channel_id>/`: Retrieve channel details.

## Installation

1. **Clone the repository**:

   git clone https://github.com/yourusername/youtube-audio-downloader.git
   cd youtube-audio-downloader

2. **Install the required Python packages**:

   pip install -r requirements.txt

3. **Run Database Migrations**:

   python manage.py migrate

4. **Start the development server**:

   python manage.py runserver

5. **Access the application**:
   Open your web browser and go to `http://localhost:8000`.

## Configuration

- **Media Files**: Ensure that the `MEDIA_ROOT` directory is set correctly in `settings.py`.
- **Download Directories**: Check the audio download directories and ensure proper permissions.
- **Tasks**: Manage background tasks using `start_background_tasks.py`.

## Usage

- **Add a Channel**: Navigate to the `Add YouTube Channel` page and input the required information.
- **Download Songs**: Use the media list to view and download available audio files.
- **Create Playlists**: Use the playlist creation form to organize your favorite tracks.

## Development

Additional logging and debugging can be configured via Django's logging settings in `settings.py`. The application also provides an admin interface to manage users and playlists.
















# FRONTEND   Song Project

## Overview

The Song Project is a frontend application built with modern web technologies, providing users with a music streaming interface reminiscent of popular platforms like Spotify. The application features functionalities such as viewing and managing playlists, browsing albums and artists, and playing songs.

## Features

- **Mock Data**: Uses mock data for songs, playlists, albums, and artists for initial setup and testing.
- **Playlists Management**: Users can create, edit, and manage playlists including adding songs and setting privacy settings.
- **Artist Pages**: View detailed artist information, including artist-specific songs and popularity.
- **Albums**: Browse through various albums with song listings.
- **Playback Functionalities**: Includes a music player with basic controls such as play, pause, next, and previous.
- **Responsive Design**: Mobile-friendly UI design using CSS/SCSS and Tailwind CSS for ensuring a seamless experience across devices.

## Mock Data

The application leverages mock data stored in `mockData.ts` which includes:

- **Songs**: Information such as `title`, `artist`, `album`, `duration`, and `popularity`.
- **Playlists**: Attributes like `name`, `description`, `songs`, `followers`, and `isPublic` status.
- **Albums**: Details including `releaseDate`, `songs`, and album-specific metadata.
- **Artists**: Artist information including `followers`, `monthlyListeners`, and associated songs.

## Functional Components

- **SongItem**: Displays individual song details with interaction capabilities.
- **ContentHeader**: Headers for playlists, artists, and albums displaying detailed metadata.
- **MusicPlayer**: Interactive music playback controls.

## API

Various asynchronous functions are provided for API interaction:

- `getSongsByArtist(channelId)`: Fetches songs for a given artist.
- `createPlaylist(data)`: Handles playlist creation with server-side submission.
- `getDownloadedSongs()`: Manages retrieval of downloaded songs.

## How to Use

1. **Installation**: Use `npm install` to install dependencies.
2. **Running Locally**: Execute `npm run dev` for local development, which runs the application in development mode.
3. **Building for Production**: Use `npm run build` to compile the application for production deployment.

## Technologies Used

- **React.js**: For the front-end component architecture.
- **TypeScript**: Provides static typing for safer JavaScript coding.
- **Tailwind CSS**: For utility-first styling methodology.
- **Framer Motion and Lucide-react**: For animations and icons, respectively.

## Contribution Guidelines

1. Fork the repository.
2. Create a new branch (`feature/foo`).
3. Commit changes (`git commit -am 'Add some foo'`).
4. Push to the branch (`git push origin feature/foo`).
5. Open a Pull Request.



