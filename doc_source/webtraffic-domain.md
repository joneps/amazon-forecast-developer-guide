# WEB\_TRAFFIC Domain<a name="webtraffic-domain"></a>

Use the WEB\_TRAFFIC domain to forecast web traffic to a web property or a set of web properties\. It supports the following dataset types\. The relevant topics describe required and optional fields the dataset type supports\. For information about how to map these fields to columns in your training data see [Dataset Domains and Dataset Types](howitworks-datasets-groups.md#howitworks-dataset-domainstypes)\.

**Topics**
+ [TARGET\_TIME\_SERIES Dataset Type](#target-time-series-type-webtraffic-domain)
+ [RELATED\_TIME\_SERIES Dataset Type](#related-time-series-type-webtraffic-domain)

## TARGET\_TIME\_SERIES Dataset Type<a name="target-time-series-type-webtraffic-domain"></a>

The following fields are required: 
+ `item_id` \(string\) – A unique identifier for each web property being forecast\.
+ `timestamp` \(timestamp\)
+ `value` \(float\) – This is the `target` field for which Amazon Forecast generates a forecast\.

Ideally, only these required fields should be included\. Other additional time series information should be included in a RELATED\_TIME\_SERIES dataset\.

## RELATED\_TIME\_SERIES Dataset Type<a name="related-time-series-type-webtraffic-domain"></a>

The following fields are required: 
+ `item_id` \(string\)
+ `timestamp` \(timestamp\)

In addition to the required fields, your training data can include other fields\. To include other fields in the dataset, provide the fields in a schema when you create the dataset\.