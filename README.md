# Install Docker Compose

This GitHub Action installs Docker Compose v2

## Usage

```yaml
jobs:
  my-awesome-job:
    steps:
      - name: Install Compose
        uses: ndeloof/install-compose-action@v0.0.1
        with:
          version: v2.1.0 # defaults to 'latest'
          legacy: true    # will also install in PATH as `docker-compose`
      - run: docker-compose --version
```
