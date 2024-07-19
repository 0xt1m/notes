# Splunk Core Cretified User
## Test Details
- 60 Questions
- Entry Level
- 60* Minutes

## Exam Contents
### Splunk Basics
1. Splunk Components +
    - Indexer
    - Search Head
    - Forwarder
    - Deployment server
    - Functions at a glance
    - Index replication and indexer clusters
2. Understand the uses of Splunk +
3. Define Splunk apps +
    - A Splunk app is an extension of Splunk functionality. Splunk apps are made up of different Splunk knowledge objects.
4. Customizing user settings +
5. Basic naviagation in Splunk +

### Basic Searching
1. Run basic searches +
2. Set the time range of a search +
3. Identify the contents of search results +
4. Refine searches +
5. Use the timeline +
6. Work with events +
7. Control a search job +
    - Each time a run a search, create a pivot, open a report or load a dashboard panel, Splunk software creates a Job in the system.
    - Jobs page to review and manage any job that you own.
    - Default lifetime of a job is 10 minutes.
    - Activity > Jobs
8. Save search results +

### Using Fields in Searches
1. Understand fields +
2. Use fields in searches +
3. Use the fields sidebar +

### Search Language Fundamentals
1. Review basic search commands and general search practices +
2. Examing the search pipeline +
3. Specify indexes in searches +
4. Use the following commands to perform searches: `table`, `rename`, `fields`, `dedup`, and `sort` +

### Using Basic Transforming Commands
1. The `top` command +
2. The `rare` command + 
3. The `stats` command +

### Creating Reports and Dashboards
1. Save a search as a report +
2. Edit reports +
3. Create reports that display statistics (table) +
4. Create repports that display visualizations (charts) +
5. Create a dashboard +
6. Add a report to a dashboard +
7. Edit a dashboard +

### Creating and Using Lookups
1. Describe lookups +
    - Lookups enrich your data by adding field-value combination from lookup tables.
2. Examine a lookup file example +
3. Create a lookup file and create a lookup definition +
    - Lookup definition - The part of the lookup configuration that defines the data type and connection parameters used when comparing event fields.
4. Configure an automatic lookup +
    - Manual lookups called with the `lookup` command
    - Automatic lookups are run everytime we run a search. "Applied to all searches at a search time."
5. Use the lookup in searches
    - To use lookup in searches we use `lookup` command

### Creating Scheduled Reports and Alerts
1. Describe scheduled reports +
2. Configure scheduled reports +
3. Describe alerts + 
4. Create alerts +
5. View fired alerts +