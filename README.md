# ArcGIS HMTL Sanitizer

This bundle adds the functionality to sanitize HTML strings to remove unsecure content.
This functionality can be used to securely use v-html in map.apps projects.

The bundle uses the ArcGIS HTML Sanitizer: [Source Repository](https://github.com/Esri/arcgis-html-sanitizer)<br>
Documentation: [Link](https://github.com/Esri/arcgis-html-sanitizer/blob/master/README.md)

## Development Guide
### Define the mapapps remote base
Before you can run the project you have to define the mapapps.remote.base property in the pom.xml-file:
`<mapapps.remote.base>http://%YOURSERVER%/ct-mapapps-webapp-%VERSION%</mapapps.remote.base>`

### Other methods to to define the mapapps.remote.base property.
1. Goal parameters
`mvn install -Dmapapps.remote.base=http://%YOURSERVER%/ct-mapapps-webapp-%VERSION%`

2. Build properties
Change the mapapps.remote.base in the build.properties file and run:
`mvn install -Denv=dev -Dlocal.configfile=%ABSOLUTEPATHTOPROJECTROOT%/build.properties`
