# Splunk

### Table of Contents {#contents}
- [Knowledge Objects](#knowledge-objects)
    - [Naming Conventions](#naming-conventions)
    - [Permissions](#permissions)


## Knowledge Objects {#knowledge-objects}
*Help you to discover and analyze your data.*

Fields
: Building blocks of the splunk search

Field extractions
: You can extract fields from raw data using regex or delimiters

Field aliases
: You can give alternate names to some fields to make your search more comfortable.

Calculated Fields
: Perform calculations based on the values of exsiting fields.

Lookups
: Additional fields can be added to your data using lookups.

Event types
: You can save your search as an Event Type.
: Provide a way to help you categorize your data.

Tags
: Save key:value pairs. Labels for data.

Workflow Actions
: Provide links within events that interact with external resources or narrow our search. 
: Use `GET` or `POST` method to pass information or pass information back to Splunk to permorm a secondary search.

Reports
: You can save searches that you run repeatedly to reports.

Alerts
: Get a notification when certain conditions are met.

Macros
: Frequently used searches saved to kind of functions where you can also pass arguments.

[Data Models](#data-model)
: Hierarchically structured datasets that can consist of three types of datasets. Events. Searches. `AND`, `OR` transactions.
: Explore data in a graphical interface.

---

### Naming Conventions {#naming-conventions}
*Help understand what each knowledge object does.*
**6 segments of keys:**
1. Group
2. Type
3. Platform
4. category
5. Time
6. Description

**Example:**
*Security-Focused Workflow Action* for *Operations team* that returns *information about user's IP*: 
```
OPS_WFA_Network_Security_na_IPwhoisAction

OPS           = Group
WFA           = Type
Network       = Platform
Security      = Category
na            = Time (not time based in this case)
IPwhoisAction = Description
```

---

### Permissions {#permissions}
Private
: When `user` creates and object it is automatically set to private. It is only available to that  user.

Specific App
: `power user`, `admin` are allowed to create knowledge objects that will be shared will all users of an app.
: Can grant roles read and write permissions.

All Apps
: `admin` is the only user role that is allowed to make knowledge objects available to all apps.
: Can grant roles read and write permissions.

---
---
---
### Data Model {#data-model}
Data Model
: A model to associate specific types to.
Data model :arrow_right: Data set :arrow_right: subset.

### CIM {#cim}
CIM
: Common Information model.
: A model. Data normalization.

### Lookup {#lookup}
Lookup
: Adding data from external sources.

---

### Transforming commands {#transforming-commands}
Transforming Commands
: Take data through `|` symbol and transform it.
- `stats`
    - `count`
    - `sum`, `avg`, `max`, `min`
    - `values`
    - `list`
    - `dc`
    - `first`, `last`
- `chart`
- `timechart`
- `top`
- `rare`
- `contingency`
- `highlight`

*Examples:*
```
index=* | stats count by purchase
```