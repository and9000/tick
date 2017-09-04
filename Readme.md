# Tick Stack

Easy to use `docker-compose.yml` file which allows you to deploy a [Tick Stack](https://www.influxdata.com/time-series-platform/) in seconds.

---

### Configuration

Every service use official image except for `telegraf` which use a customized `Dockerfile`: I've added `python3` and some pip packages I required.  

Configuration for various services are stored in `docker_data/$service_name/config`.

Data directory for various services are stored in `docker_data/$service_name/data`.

### Usage

Clone the repository, start with `docker-compose up` and point a browser to [http://localhost:8888/](http://localhost:8888/).

### License

Copyright &copy; 2017 Andrea Lorenzetti (<andrea@lorenzetti.me>)

Released under the terms of the [GNU General Public License, version 3](https://gnu.org/licenses/gpl.html)

