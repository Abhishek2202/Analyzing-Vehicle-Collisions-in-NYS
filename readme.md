**Motor Vehicle Crashes**

Members

Abhishek Gupta (guptaa10)
Harsh Sugandh (suganh)

**Downloading the Datasets**

All the required datasets can be found in the GitHub repository under the folder "Dataset".

**Setting up the System**

Postgres

Login as 'Postgres' using
psql -U postgres

After logging in run the following code:

CREATE USER dmvadmin WITH PASSWORD 'dmvadmin';
CREATE DATABASE motorvehiclecrashes;
GRANT ALL PRIVILEGES ON DATABASE motorvehiclecrashes TO dmvadmin;

Use \q or \quit to exit and the Schema can be created using

psql -U dmvadmin motorvehiclecrashes < Schema.sql

**Loading the data**

The following Python package is required: pip install psycopg2, pip install psycopg2.extras

The data can be loaded by running 'load_data.py' available in the GitHub repository.