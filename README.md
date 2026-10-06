# Oracle PDB Assignment II - 25401 Fumba

This project documents the creation of an Oracle Pluggable Database (PDB) in a local Oracle 21c environment. The screenshots below show the database connection details and the SQL command used to create the PDB successfully.

## Project Overview

The goal of this assignment was to create a new pluggable database inside an Oracle container database and confirm the setup with the required connection information. The database used for this task was configured as follows:

- Username: FUMBA_PLSQLAUCA_25401
- Password: The new password you just set
- Hostname: localhost
- Port: 1521
- Service Name: fu_pdb_25401
- Role: default
- Connection Type: Basic

## Connection Details

The first screenshot below shows the Oracle connection configuration used to connect to the database instance.


</p>

## Process Followed

The process used to create the PDB was:

1. Open SQL*Plus as SYSDBA.
2. Connect to the Oracle instance using the local database credentials.
3. Run the CREATE PLUGGABLE DATABASE command with an administrator user.
4. Confirm that the database was created successfully.

The command shown in the screenshot was:

```sql
CREATE PLUGGABLE DATABASE fu_pdb_25401
ADMIN USER FUMBA_plsqlauca_25401 IDENTIFIED BY YourPassword;
```

The result returned by Oracle was:

```text
Pluggable database created.
```

## Screenshot of the PDB Creation

This screenshot shows the SQL*Plus session where the PDB was created successfully.

<p align="center">
  <img src="screenshots/created%20(1).jpeg" alt="SQL*Plus creating the Oracle pluggable database" width="1000" />
</p>

## Result

The Oracle database instance was successfully configured with a new pluggable database named `fu_pdb_25401`, and the creation was confirmed through the SQL*Plus output. This completed the required PDB setup task for the assignment.

## Notes

- The database was created locally using Oracle 21c.
- The PDB name and admin user match the values shown in the connection details and SQL command screenshots.
- The screenshots in this repository serve as evidence of the completed process.
