So I am currently setting to set up a monitoring dashboard for a [Docker](https://www.docker.com/)-host using [cAdvisor](https://github.com/google/cadvisor), [Grafana](http://grafana.org/) and [Prometheus](https://prometheus.io/).

Since I couldn't find any proper documentation of the exposed metrics, I decided to just take the info from the /metrics entpoints and bring it into a human-readable format.

Maybe I can save someone a couple of minutes.

When building Graphs/Dashboards with Grafana, knowing the data storage's query dsl and metric types is important. Documentation about using Grafana with an InfluxDB won't help you much if your storage backend is Prometheus, which is kind of unfortunate. Anyways here you can find the official documentation for Prometheus:

[Information on Prometheus Metric Types](https://prometheus.io/docs/concepts/metric_types/)  
[Information on Prometheus Querying](https://prometheus.io/docs/querying/basics/)  

Versions:  
cAdvisor: 0.23.1  
Prometheus: 0.16.1  
[Node-Exporter](https://github.com/prometheus/node_exporter): 0.12.0
