# Django Chat Application

A real-time chat application built with Django, PostgreSQL, and Redis. This application provides a modern messaging platform with real-time updates using WebSocket connections.

## Features

- Real-time messaging using WebSocket
- User authentication and authorization
- Message history
- Online user status
- Modern and responsive UI
- Docker support for easy deployment

## Tech Stack

- **Backend**: Django 3.1
- **Database**: PostgreSQL 13
- **Cache/Messaging**: Redis 6
- **WebSocket**: Django Channels
- **Containerization**: Docker & Docker Compose

## Prerequisites

- Docker and Docker Compose
- Git

## Installation

1. Clone the repository:
```bash
git clone https://github.com/VoroninEgor/uoykaii-chat.git
cd uoykaii-chat
```

2. Build and start the containers:
```bash
docker-compose up --build
```

The application will be available at `http://localhost:8000`

## Development Setup

1. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install pipenv
pipenv install
```

3. Run migrations:
```bash
python manage.py migrate
```

4. Start the development server:
```bash
python manage.py runserver
```

## Docker Services

The application consists of three main services:

- **Web**: Django application server
- **PostgreSQL**: Database server
- **Redis**: Cache and message broker

## Environment Variables

The following environment variables are used in the application:

- `POSTGRES_DB`: Database name (default: chat)
- `POSTGRES_USER`: Database user (default: postgres)
- `POSTGRES_PASSWORD`: Database password
- `REDIS_URL`: Redis connection URL

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Author

Egor Voronin
