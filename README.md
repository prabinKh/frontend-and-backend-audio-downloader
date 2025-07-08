# Song Project

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

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
