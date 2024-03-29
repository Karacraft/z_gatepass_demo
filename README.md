## Application Details
|               |
| ------------- |
|**Generation Date and Time**<br>Tue Mar 26 2024 08:49:06 GMT+0500 (Pakistan Standard Time)|
|**App Generator**<br>@sap/generator-fiori-elements|
|**App Generator Version**<br>1.12.3|
|**Generation Platform**<br>Visual Studio Code|
|**Template Used**<br>List Report Page V2|
|**Service Type**<br>OData Url|
|**Service URL**<br>http://192.168.10.45:8000/sap/opu/odata/sap/Z_C_GPHEADER_CDS
|**Module Name**<br>z_gatepass_demo|
|**Application Title**<br>Manage Gatepass|
|**Namespace**<br>com.tl.gp|
|**UI5 Theme**<br>sap_horizon|
|**UI5 Version**<br>1.108.22|
|**Enable Code Assist Libraries**<br>False|
|**Enable TypeScript**<br>False|
|**Add Eslint configuration**<br>False|
|**Main Entity**<br>Z_C_GPHEADER|
|**Navigation Entity**<br>to_items|

## z_gatepass_demo

Manage Gatepass &amp; Line Items

### Starting the generated app

-   This app has been generated using the SAP Fiori tools - App Generator, as part of the SAP Fiori tools suite.  In order to launch the generated app, simply run the following from the generated app root folder:

```
    npm start
```

- It is also possible to run the application using mock data that reflects the OData Service URL supplied during application generation.  In order to run the application with Mock Data, run the following from the generated app root folder:

```
    npm run start-mock
```

#### Pre-requisites:

1. Active NodeJS LTS (Long Term Support) version and associated supported NPM version.  (See https://nodejs.org)  


Actual Data  
~~~js
 "sap.ui.generic.app": {
    "_version": "1.3.0",
    "settings": {
      "forceGlobalRefresh": false,
      "objectPageHeaderType": "Dynamic",
      "considerAnalyticalParameters": true,
      "showDraftToggle": false,
      "flexibleColumnLayout": {
        "defaultTwoColumnLayoutType": "TwoColumnsMidExpanded",
        "defaultThreeColumnLayoutType": "ThreeColumnsEndExpanded"
      }
    },
    "pages": {
      "ListReport|Z_C_GPHEADER": {
        "entitySet": "Z_C_GPHEADER",
        "component": {
          "name": "sap.suite.ui.generic.template.ListReport",
          "list": true,
          "settings": {
            "condensedTableLayout": true,
            "smartVariantManagement": true,
            "enableTableFilterInPageVariant": true,
            "filterSettings": {
              "dateSettings": {
                "useDateRange": true
              }
            }
          }
        },
        "pages": {
          "ObjectPage|Z_C_GPHEADER": {
            "entitySet": "Z_C_GPHEADER",
            "defaultLayoutTypeIfExternalNavigation": "MidColumnFullScreen",
            "component": {
              "name": "sap.suite.ui.generic.template.ObjectPage"
            },
            "pages": {
              "ObjectPage|to_items": {
                "navigationProperty": "to_items",
                "entitySet": "Z_C_GPITEMS",
                "defaultLayoutTypeIfExternalNavigation": "MidColumnFullScreen",
                "component": {
                  "name": "sap.suite.ui.generic.template.ObjectPage"
                }
              }
            }
          }
        }
      }
    }
  },
~~~