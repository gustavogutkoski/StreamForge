# StreamForge

StreamForge is an open-source project designed to provide a modular and scalable video streaming platform.  
The goal is to create a system where each component — such as the API, transcoding service, and frontend — is developed as an independent service, but can also work seamlessly together as a complete solution.

## Project Structure

The project is organized as a parent repository that aggregates submodules for each service:
```
StreamForge
    ├── streamforge-api # Backend API (CRUD, database integration, user/video management)
    ├── streamforge-transcoder # Service for video transcoding (TODO)
    ├── streamforge-frontend # Frontend application (TODO)
```

Each submodule has its own lifecycle, dependencies, and deployment strategy, but all can be orchestrated together.

## Getting Started

To clone the repository with all its submodules:

```bash
    git clone --recurse-submodules https://github.com/gustavogutkoski/StreamForge.git
```

If you already cloned it without submodules, you can initialize and update them with:
```bash
    git submodule update --init --recursive
```

## License

This project is licensed under the MIT License. See the LICENSE file for details.