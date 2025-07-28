# EspoCRM + Mautic Integration Platform

A comprehensive integration platform that unifies EspoCRM and Mautic with a modern admin console for seamless CRM and marketing automation management.

## Features

- **Unified Admin Console**: Modern React-based dashboard for managing both platforms
- **Bidirectional Sync**: Automatic synchronization of contacts and campaigns
- **Real-time Analytics**: Comprehensive reporting and insights
- **API Integration**: RESTful APIs for both EspoCRM and Mautic
- **Docker Deployment**: Complete containerized solution
- **Monitoring & Logging**: Built-in sync monitoring and error tracking

## Quick Start

### Prerequisites
- Docker and Docker Compose
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Tiya254/crm-marketing-integration.git
   cd crm-marketing-integration
   ```

2. **Configure environment variables**
   ```bash
   cp .env.example .env
   # Edit .env with your specific configuration
   ```

3. **Start the services**
   ```bash
   docker-compose up -d
   ```

4. **Access the applications**
   - Admin Console: http://localhost:3000
   - EspoCRM: http://localhost:8080
   - Mautic: http://localhost:8081
   - Integration API: http://localhost:5000

## Architecture

### Backend Services
- **Integration API**: .NET 8 Web API for orchestrating integrations
- **EspoCRM Service**: Handles EspoCRM API interactions
- **Mautic Service**: Manages Mautic OAuth2 and API calls
- **Sync Service**: Automated data synchronization engine
- **Analytics Service**: Data analysis and reporting

### Frontend
- **Admin Console**: Next.js 14 with TypeScript and Tailwind CSS
- **Dashboard**: Real-time metrics and system status
- **Contact Management**: Unified contact view across platforms
- **Campaign Management**: Cross-platform campaign oversight
- **Sync Monitoring**: Live sync status and logs
- **Settings**: Configuration management interface

### Infrastructure
- **EspoCRM**: Open-source CRM platform
- **Mautic**: Marketing automation platform
- **MySQL**: Database for all services
- **Redis**: Caching and session management
- **Docker**: Containerized deployment

## License

This project is licensed under the MIT License.
