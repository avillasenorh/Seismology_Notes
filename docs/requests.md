# Data

## Data requests with FDSNWS

Description of FDSN web services: [web](http://service.iris.edu/fdsnws/).

- [availability](http://service.iris.edu/fdsnws/availability/1/):
  returns detailed time span information of what timeseries data is available at the archive.

- [station](http://service.iris.edu/fdsnws/station/1/):
  returns station metadata in FDSN StationXML format or as delimited text.

- [dataselect](http://service.iris.edu/fdsnws/dataselect/1/):
  provides access to time series data for specified channels and time ranges.

- [event](http://service.iris.edu/fdsnws/event/1/):
   returns event (earthquake) information from catalogs originating from the NEIC and the ISC data centers.

Most services also have a web interface to build URLs for data request.
For example, for the [IGN](https://www.ign.es/) web service:

    http://193.144.251.72:8080/fdsnws/station/1/builder

To request all responses:

    http://193.144.251.72:8080/fdsnws/station/1/query?level=response&formatted=true&nodata=404
