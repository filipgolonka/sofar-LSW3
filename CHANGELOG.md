# Change Log
Get Sofart Inverter's data from solarman logger.
Tested with LSW-3 (SN 17xxxxxxx, 21xxxxxx)
 
## [1.0] - 2021-09-22
Clone whole project from github and put in crontab to run in intervals.

### Added
1. Sofar Inverter support.
2. Language support (Polish, English).
3. Cleaned SOFARMap.xml file.
 
### Changed
 
### Fixed

## [1.1] - 2021-09-23
To upgrade overwrite all previous project files.
To use prometheus+graphana support:
1. Configure prometheus options in config.cfg
2. Serve prometheus metrics file using any web server (name it index.html to be the default page in configured path)
3. Configure prometheus target to access the file
4. Add Prometheus datasource in Grafana
5. Import grafana_en/pl.json file (Dashboards->Manage->Import).
Enjoy :)

### Added
1. Prometheus + grafana support.
2. Verbose mode.
 
### Changed
 
### Fixed
1. 4-byte values (Total production, Total generation time) calculated correctly.