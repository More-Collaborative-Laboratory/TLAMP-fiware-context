# Organization

Describes the organization entity
-  `id`: Organization Identifier
   -  Attribute type: **Property**. 
   -  Required
-  `legalName`: Organization's legal name
   -  Attribute type: **Property**. [legalName](https://schema.org/legalName)
   -  Required
-  `taxId`: The organization's tax number
   -  Attribute type: **Property**. [taxID](https://schema.org/taxID)
   -  Required
-  `dateCreated`: Date that the Organization was Created in data base.
   -  Attribute type: **Property**. [](https://schema.org/dateCreated/)
   -  Optional
-  `dateModified`: Date that any information about Organization was modified.
   -  Attribute type: **Property**. [](https://schema.org/dateModified/)
   -  Optional
-  `email`: Contact email address
   -  Attribute type: **Property**. [email](https://schema.org/email)
   -  Required
-  `telephone`: Mobile or telephone contact
   -  Attribute type: **Property**. [telephone](https://schema.org/telephone)
   -  Required
-  `address`: The company's headquarters address
   -  Attribute type: **Property**. [address](https://schema.org/address)
   -  Optional
-  `url`: Oganization Web Site
   -  Attribute type: **Property**. [url](https://schema.org/url)
   -  Optional
-  `location`: Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon
   -  Attribute type: **GeoProperty**. 
   -  Optional



# Field

Field Entity for T-LAMP Project.
-  `id`: Field UUID
   -  Attribute type: **Property**. 
   -  Optional
-  `address`: The company's headquarters address
   -  Attribute type: **Property**. [address](https://schema.org/address)
   -  Optional
-  `category`: The categories that this building belongs to
   -  Attribute type: **EnumProperty**. 
   -  Optional
-  `dateCreated`: Date that the Organization was Created in data base.
   -  Attribute type: **Property**. [](https://schema.org/dateCreated/)
   -  Optional
-  `dateModified`: Date that any information about Organization was modified.
   -  Attribute type: **Property**. [](https://schema.org/dateModified/)
   -  Optional
-  `ownedBy`: Relationship to Organization, this devices is ownedBy: urn:ngsi-ld:Organization:Organization_UUID.
   -  Attribute type: **Relationship**. 
   -  Optional
-  `seedType`: The seed types used in the current field
   -  Attribute type: **Property**. [Text](https://schema.org/Text)
   -  Optional
-  `fieldWidth`: 
   -  Attribute type: **Property**. [serialNumber](https://schema.org/serialNumber)
   -  Optional
-  `fieldHeight`: 
   -  Attribute type: **Property**. [serialNumber](https://schema.org/serialNumber)
   -  Optional
-  `location`: Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon
   -  Attribute type: **Geoproperty**. 
   -  Optional



# Treatment

Describes the treatment entity
-  `id`: Organization Identifier
   -  Attribute type: **Property**. 
   -  Optional
-  `treatmentState`: The treatment state, there are. One of : `wainting`, `ongoing`, `paused`, `finished`.
   -  Attribute type: **Property**. 
   -  Optional
-  `begin`: DateTime that the treatment REALY begun
   -  Attribute type: **Property**. [Schedule](https://schema.org/Schedule)
   -  Optional
-  `estimatedBegin`: DateTime to estimate a begin to treatment
   -  Attribute type: **Property**. [Schedule](https://schema.org/Schedule)
   -  Optional
-  `duration`: Tthe REAL durantion of the treatment
   -  Attribute type: **Property**. [Schedule](https://schema.org/Schedule)
   -  Optional
-  `estimatedDuration`: Tthe REAL durantion of the treatment
   -  Attribute type: **Property**. [Schedule](https://schema.org/Schedule)
   -  Optional
-  `radius`: The radius to create an area for the treatment
   -  Attribute type: **Property**. [Number](https://schema.org/Number)
   -  Optional
-  `treatmentType`: The treatment type
   -  Attribute type: **Property**. [Text](https://schema.org/Text)
   -  Optional
-  `location`: Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon
   -  Attribute type: **Geoproperty**. 
   -  Optional



# Profile

Profile Entity for T-LAMP Project.
-  `id`: Profile UUID
   -  Attribute type: **Property**. 
   -  Optional
-  `predefined`: Predefined value to actuate in the LED and IR channels. One of : `predefined 1`, `predefined 2`, `predefined 3`, `predefined 4`, `predefined 5`.
   -  Attribute type: **Property**. 
   -  Optional
-  `seedType`: The seed types used in the current field
   -  Attribute type: **Property**. [Text](https://schema.org/Text)
   -  Optional
-  `channelsInProfile`: This create an array to send command to the channel in order to  control the channels. See the file How to Send data to Control the Channels.js in the PATH: OneDrive../T-LAMP/_EXECUCAO/
   -  Attribute type: **Property**. 
   -  Optional



# Car

Car Device for T-LAMP Project.
-  `id`: Car UUID
   -  Attribute type: **Property**. 
   -  Optional
-  `ownedBy`: Relationship to Organization, this devices is ownedBy: urn:ngsi-ld:Organization:Organization_UUID.
   -  Attribute type: **Relationship**. 
   -  Optional
-  `deviceState`: State of this device from an operational point of view. Its value can be vendor dependent.
   -  Attribute type: **Property**. [Text](https://schema.org/Text)
   -  Optional
-  `serialNumber`: The serial number assigned by the manufacturer.
   -  Attribute type: **Property**. [serialNumber](https://schema.org/serialNumber)
   -  Optional
-  `usedBy`: Relationship to a Treatment, this Device is usedBy the Treatment Entity to retrive data
   -  Attribute type: **Relationship**. 
   -  Optional
-  `supportedProtocol`: This will differentiate a Car Master ( LTE ) or Car Slave ( BLE ).
   -  Attribute type: **EnumProperty**. 
   -  Optional
-  `location`: Geoproperty. Geojson reference to the item. Point
   -  Attribute type: **GeoProperty**. 
   -  Optional
-  `voltage`: Car Voltage value corresponding to this observation.
   -  Attribute type: **Property**. [Number](https://schema.org/Number)
   -  Optional
-  `powerConsumption`: Power consumed by the Car.
   -  Attribute type: **Property**. [Number](https://schema.org/Number)
   -  Optional
-  `powerFactor`: Power factor or the ratio of working power of the Car corresponding to this observation.
   -  Attribute type: **Property**. [Number](https://schema.org/Number)
   -  Optional
-  `frequency`: Car's voltage frequency observed.'
   -  Attribute type: **Property**. [Number](https://schema.org/Number)
   -  Optional
-  `channelsInTheCar`: This create an array to send command to the channel in order to  control the channels. See the file How to Send data to Control the Channels.js in the PATH: OneDrive../T-LAMP/_EXECUCAO/
   -  Attribute type: **Property**. 
   -  Optional



# Sensor

Sensor Node for T-LAMP Project.
-  `id`: Sensor Node UUID
   -  Attribute type: **Property**. 
   -  Required
-  `ownedBy`: Relationship to Organization, this devices is ownedBy: urn:ngsi-ld:Organization:Organization_UUID.
   -  Attribute type: **Relationship**. 
   -  Required
-  `batteryLevel`: Device battery level. It must be equal to 100.0 when battery is full. 0.0 when battery is empty. -1 when transiently cannot be determined.
   -  Attribute type: **Property**. [Number](https://schema.org/Number)
   -  Required
-  `deviceState`: State of this device from an operational point of view. Its value can be vendor dependent.
   -  Attribute type: **Property**. [Text](https://schema.org/Text)
   -  Required
-  `serialNumber`: The serial number assigned by the manufacturer.
   -  Attribute type: **Property**. [serialNumber](https://schema.org/serialNumber)
   -  Required
-  `usedBy`: Relationship to a Treatment, this Device is usedBy the Treatment Entity to retrive data
   -  Attribute type: **Relationship**. 
   -  Required
-  `quantum`: PAR Measured by SQ-521 (umol/m^-2/s^-1) - OBS: The UNIT CODE is not available, it is under review by UN/CEFACT
   -  Attribute type: **Property**. 
   -  Optional
-  `soilHumidity`: Soil Humidity measured by SMTEC
   -  Attribute type: **Property**. 
   -  Optional
-  `soilTemperature`: Soil Temperature measured by SMTEC
   -  Attribute type: **Property**. 
   -  Optional
-  `soilConductivity`: Soil Electric Conductivity measured by SMTEC
   -  Attribute type: **Property**. 
   -  Optional
-  `soilPh`: Soil pH measured by pH sensor
   -  Attribute type: **Property**. 
   -  Optional
-  `airHumidity`: Air Humidity measured by BME280
   -  Attribute type: **Property**. 
   -  Optional
-  `airTemperature`: Air Temperature measured by BME280
   -  Attribute type: **Property**. 
   -  Optional
-  `location`: Geoproperty. Geojson reference to the item. Point
   -  Attribute type: **GeoProperty**. 
   -  Optional



## Examples

### OK


