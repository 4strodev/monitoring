# Monitoring
This is a toy application designed to practice application monitoring made with go. The main tools for this purpouse are:

- [slog](https://pkg.go.dev/log/slog): The go std library package for structured logging
- [loki](https://grafana.com/oss/loki/): The grafana solution for logs processing
- [alloy](https://grafana.com/oss/alloy/): The client designed to scrap and send logs to loki
- [grafana](https://grafana.com/): The panel to connect with loki and view logs

## Start project
The recomended way is using docker compose.

    docker compose up -d

Then you will be able to interact with different services. But the most important ones are. The application itself
and the grafana dashboard.

- [Application](http://localhost:8080): Just play with the app to start triggering events.
- [Grafana](http://localhost:3000): Go to the explore section to start viewing logs. Recommended to have
knowledge of logql.

## Featuers
This app is just a simple app that allows you to login and create some data. The main point here is how the tools are
connected to allow monitoring of your application.

