# WPQuery

WPQuery enables external access to the internal database structure of a Wordpress instance.

This can be useful when migrating from Wordpress to a different platform, or when a third party needs to integrate with a Wordpress based site.

When installed the db structures of Worpdress can be exposed via wp-json. 

The plugin generates a unique API key, which can the be used to access this data.

## Usage

### List all database tables for the Wordpress installation:

http://localhost/wp-json/wpquery/v1/query?apikey={API_KEY}

### List all rows for a given table:

http://localhost/wp-json/wpquery/v1/query/{TABLE}?apikey={API_KEY}

### Get a row by the primary key of the table:

http://localhost/wp-json/wpquery/v1/query/{TABLE}/{ID}?apikey={API_KEY}

### Get a row by the given key value:

http://localhost/wp-json/wpquery/v1/query/{TABLE}/{KEY}/{VALUE}?apikey={API_KEY}
