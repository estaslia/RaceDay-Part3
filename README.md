# RaceDay - Event Management System (Part 3)

This is the Part 3 submission for the RaceDay platform. It consists of an ASP.NET Core MVC Web Application that consumes the Part 2 API.

## Features
- **Authentication**: Login and Register via the API.
- **Organiser Dashboard**: Create events, upload banner images to Azure Blob Storage, and capture participant results.
- **Participant Interface**: Browse upcoming events, enrol in categories, and view personal race history (My Races).
- **Azure Blob Storage**: Event banner images are uploaded and stored via the API.
- **UI**: Built with Bootstrap 5, responsive, and role-based navigation.

## Prerequisites
- .NET 8.0 SDK
- Docker Desktop (for containerization)
- The Part 2 API must be running on `https://localhost:7100`

##  Docker Setup

To run the MVC application inside a Docker container, use the following commands.

**1. Build the Docker image:**
Run this command from the root directory (where the `.sln` file is located):
```bash
docker build -t raceday-mvc -f RaceDay.MVC/Dockerfile .