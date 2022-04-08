## Mobile Settings

The Mobile Settings widget allows users to customize their mobile user interface. The user can manipulate the UI using one of the following three JSON files:
*	navigation.json – can be used to edit the navigation menu
*	listView.json – can be used to edit the module list view
*	detailView.json – can be used to edit the module detail view

**Certified**: Yes  

**Publisher**: Fortinet  

**Compatibility**: 7.0.2 or higher

**Applicable**: Widget Library

**Widget Details**:  

<h3 style="border-bottom: 1.8px solid gray;"> navigation.json</h3></br>

**File Path**: widgetAssets/navigation.json  

The **navigation.json** file contains the ` navigation_list` key, which is an array of three objects:  
*	Incident Response
*	Threat Intelligence
*	Vulnerability Management

Each object contains the following parameters:

| Parameter     | Description          |
| -------- | -------------- |
| label | Label of the navigation element |
| icon | Icon of the navigation element |
| modules | Array of module objects nested in the navigation element |
| modules.type | Type of module |
| modules.label | Label of the module |
| modules.icon | Icon of the module |
| modules.default | If true, that particular module will open once the user logs in. |
| modules.primary | If true, that particular module will be the primary module of the navigation element. |

The **navigation.json** renders as follows in the UI:

<img src="https://raw.githubusercontent.com/fortinet-fortisoar/widget-mobile-settings/release/2.0.0/docs/media/mobile-settings-navigation.png" alt="Mobile Settings - Navigation" style="border: 1px solid #A9A9A9; border-radius: 4px; padding: 10px; display: block; margin-left: auto; margin-right: auto; width: 80%">
</br>

<h3 style="border-bottom: 1.8px solid gray;"> listView.json</h3></br>

**File Path**: \<module>/listView.json  

The **listView.json** file contains the following parameters:
| Parameter     | Description          |
| -------- | -------------- |
| primaryField | Represents the color code of the attack corresponding to its severity. |
| titleFields | The fields passed as values will be displayed as the title of the record. For example, the title can be the ID of the record and the name of the record. |
| widgets | Array of row widget objects. |
| widgets.row | The fields passed as values will be displayed in this row. For example, the row can contain who the record has been assigned to and the created date of the record. |

The **listView.json** renders as follows in the UI:

<img src="https://raw.githubusercontent.com/fortinet-fortisoar/widget-mobile-settings/release/2.0.0/docs/media/mobile-settings-list.png" alt="Mobile Settings - List View" style="border: 1px solid #A9A9A9; border-radius: 4px; padding: 10px; display: block; margin-left: auto; margin-right: auto; width: 80%">
</br>

<h3 style="border-bottom: 1.8px solid gray;"> detailView.json</h3></br>

**File Path**: \<module>/detailView.json

The **detailView.json** file contains the following parameters:

| Parameter     | Description          |
| -------- | -------------- |
| primaryField | Represents the color code of the attack corresponding to its severity. |
| titleFields | The fields passed as values will be displayed as the title of the record. For example, the title can be the ID of the record and the name of the record. |
| headerWidgets | Displays the record information of the corresponding fields in the header section.  |
| bodyWidgets | Displays the details of a particular record. The details of the record are contained in the label and column fields. |

The **detailView.json** renders as follows in the UI:

<img src="https://raw.githubusercontent.com/fortinet-fortisoar/widget-mobile-settings/release/2.0.0/docs/media/mobile-settings-detail.jpg" alt="Mobile Settings - Detail View" style="border: 1px solid #A9A9A9; border-radius: 4px; padding: 10px; display: block; margin-left: auto; margin-right: auto; width: 80%">
</br>
