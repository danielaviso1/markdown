Environment URL
---|---
Dev|https://ubpdev.appiancloud.com/suite/webapi/btq/libraries/branch/directory
Test|https://ubptest.appiancloud.com/suite/webapi/btq/libraries/branch/directory
Prod|https://ubp.appiancloud.com/suite/webapi/btq/libraries/branch/directory
---

**Sample Request**

```curl
curl -X GET \
  https://ubpdev.appiancloud.com/suite/webapi/btq/libraries/branch/directory \
  -H 'Authorization: Basic ZGRhdmlzb0B1bmlvbmJhbmtwaC5jb206YXBwaWFuZ29kMA==' \
  -H 'Postman-Token: 6a51a79f-f7bd-4d1f-add9-010368910941' \
  -H 'cache-control: no-cache'
```

**Sample Response**

```json
{
  "branchDetails" : [ {
    "solId" : "059",
    "name" : "Plaza",
    "email" : "ubp.ubplaza@unionbankph.com",
    "counterCount" : 4,
    "isTransformed" : true,
    "dqsEnabled" : true,
    "isOpen" : true,
    "isBCP" : false,
    "mobileNumber" : "09178270559 ",
    "landlineNumber" : "6341602; 6347907; 5851019; 6337929",
    "UBPRegion" : "ORTIGAS CBD",
    "geographicRegion" : "NCR",
    "rsoo" : "Dennies A. Bico",
    "rsooEmail" : "dabico@unionbankph.com",
    "rsooMobile" : "(0917) 5020867",
    "branchAddress" : "UnionBank Plaza Bldg., Meralco Ave. corner Onyx St., Pasig City",
    "latitude" : "14.587136",
    "longitude" : "121.063574",
    "parkingLots" : "common",
    "weekDayOpeningHour" : "09:00:00 AM",
    "weekDayClosingHour" : "16:00:00 PM",
    "saturdayOpeningHour" : "N/A",
    "saturdayClosingHour" : "N/A",
    "sundayOpeningHour" : "",
    "sundayClosingHour" : "",
    "localHolidays" : "N/A",
    "servicingStatus" : "N/A",
    "effectiveDate" : "N/A",
    "networkPort" : "N/A",
    "networkConnectivityStatus" : "N/A",
    "transformationTag" : "Transformed",
    "isMegaBranch" : true
  } ]
}
```

#Query Parameters 

### Batchsize
Returns first 20 branches
```batchSize
GET /branch/directory?batchSize=20
```

### Sol ID Filter
Returns branch data filtered by given Sol ID
```solId
GET /branch/directory?solid=059
```