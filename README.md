# base-elixir-phoenix-template

References
- https://medium.com/swlh/use-docker-to-create-an-elixir-phoenix-development-environment-e1a81def1d2e
- https://tailwindcss.com/docs/guides/phoenix

Template for an app with the ff dependencies:
- Phoenix 1.6.6
- Elixir
- LiveView

All contained in a docker container

# Initialization
- delete pgdata folder
- docker-compose build
- docker-compose run --rm phoenix mix deps.get
- docker-compose run --rm phoenix mix ecto.create
- docker-compose up

# Key files and changes from scratch
- Dockerfile (all)
- docker-compose.yml (all)
- dev.exs (hostname: "db", http: [ip: {0, 0, 0, 0}, port: 4000])
