# Get car details

<div class="method method-get">GET</div> <span class="url">https://app.ewill.io/server/api/customers/me/getCarDetails/{registrationNumber}</span>

> Get car details using registration number

### Parameters in URL

|Name|Description|Type|Required|
| --- | --- | --- |
| `registrationNumber` | Car registration number | `string` | <div class="required">*</div> |


### Response Example

```json
{
    "DateOfLastUpdate": "2011-01-01T00:00:00",
    "Colour": "BLACK",
    "VehicleClass": "Car",
    "EngineNumber": "XXXXXXXXXXXXXXXXX",
    "EngineCapacity": "4197",
    "TransmissionCode": "A",
    "DtpMakeCode": "B2",
    "Exported": false,
    "YearOfManufacture": "2005",
    "Scrapped": false,
    "Transmission": "AUTO 6 GEARS",
    "DateFirstRegisteredUk": "2005-06-21T00:00:00",
    "Model": "RANGEROVER SPT V8SC STD A",
    "GearCount": 6,
    "ImportNonEu": false,
    "DtpModelCode": "350",
    "GrossWeight": 0,
    "DoorPlanLiteral": "ESTATE",
    "MvrisModelCode": "AMS",
    "Vin": "XXXXXXXXXXXXXXXXX",
    "Vrm": "XXXXX",
    "DateFirstRegistered": "2005-01-01T00:00:00",
    "DoorPlan": "06",
    "VinLast5": "XXXXX",
    "VehicleUsedBeforeFirstRegistration": false,
    "MaxPermissibleMass": 3125,
    "Make": "LAND ROVER",
    "MakeModel": "LAND ROVER RANGEROVER SPT V8SC STD A",
    "TransmissionType": "Automatic",
    "SeatingCapacity": 5,
    "FuelType": "PETROL",
    "Co2Emissions": 374,
    "Imported": false,
    "MvrisMakeCode": "B2"
}
```

### Response Messages

* `200` Success
* `401` Authorization required
* `500` Error
