# ![LOGO](logo.png) Mobility **flow**ground Connector

## Description

A generated **flow**ground connector for the Mobility API (version 1.2.0).

Generated from: https://api.apis.guru/v2/specs/o2.cz/mobility/1.2.0/swagger.json<br/>
Generated at: 2019-05-07T17:43:21+03:00

## API Description

Transit API can be used to obtain time-aggregated data representing moving the people between various spatial points within the Czech Republic. Having A - 'from' and B - 'to' points, the API can return count of people traveling from A to B or people that are from A and traveling to B, etc. The mobility data is based on moving mobile stations in O2 mobile network.

## Authorization

This API does not require authorization.

## Actions

### Information about versions of application and data.

*Tags:* `info`

### Transit between basic residential units

> Get count of objects that were moving between basic residential units or objects that were visiting these basic residential units. Specific object's occurence type in the base residential unit can be requested. If none occurence type is present in the request or both occurence types are zero, the result will be aggregation of all types of occurence for given base residential units. More about base residential units can be found at https://www.czso.cz/csu/rso/zsj_rso (czech).

*Tags:* `transit`

#### Input Parameters
* `from` - _required_ - source basic residential unit
* `to` - _required_ - destination basic residential unit
* `fromType` - _optional_ - occurence type in the source basic residential unit (1 - transit, 2 - visit, 0 - both)
* `toType` - _optional_ - occurence type in the destination basic residential unit (1 - transit, 2 - visit, 0 - both)
* `uniques` - _required_ - all or only uniques (0 - all, 1 - uniques)

## License

**flow**ground :- Telekom iPaaS / o-2-cz-mobility-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
