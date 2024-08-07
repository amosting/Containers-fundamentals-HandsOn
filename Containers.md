# Containers
## Docker
### Data in containers
- Containers are ephemerous and stateless
- Non-persistent data
  - Stored within container inside memory temp file systems
  - When container is destroyed, data is destoryed along with it
- Persistent data
  - Stored outside the container in a Volume
  - Volume is mapped to a logical folder

### Docker Compose
Docker Compose is a tool for defining and running multi-container applications.
- Simplifies control of entire application stack. Makes it easy to manage services, networks and volumes in a single YAML config file
- Use cases:
  - Workloads that don't require a full orchestrator
  - Development and tests

#### Docker Compose Commands
- `docker compose build`: build the services defined in a docker-compose.yml file
- `docker compose ps`:  lists containers for a Compose project, along with their current status and exposed ports
