# <img src="https://github.com/iqp-samples/iqp-samples-ws/raw/master/logo.png" alt="iQuipsys Logo" width="100px" height="100px"> SQL Server integration sample

This is a sql server integraion sample for [IQuipsys Positron](http://www.iquipsys.com).
This sample demonstrates how to use SQL server integration services and create pivot table object presence in site zones on SQL Server.

## Installation

- Install **SQL Server Data Tools**(SSDT). This is a powerfull development tool based on Visual Studio shell.

- Clone this repository to local disk
```bash
> git clone https://github.com/iqp-samples/iqp-samples-integration-sqlserver.git
```

## Usage

- Set the login, password and all report parameters such as siteName, startDate, endDate in 'Parameters' tab

<img src="https://raw.githubusercontent.com/iqp-samples/iqp-samples-integration-sqlserver/master/img/control_flow.jpg" alt="start window">

<img src="https://raw.githubusercontent.com/iqp-samples/iqp-samples-integration-sqlserver/master/img/parameters.jpg" alt="parameters">

- Set the SQL Server connection 
<img src="https://github.com/iqp-samples/iqp-samples-integration-sqlserver/blob/master/img/sql%20server%20settings%201.jpg" alt="parameters">
<img src="https://github.com/iqp-samples/iqp-samples-integration-sqlserver/blob/master/img/sql%20server%20settings%202.jpg" alt="parameters">

    - If you don't have configured connection press 'New' and set SQL Server name and database
    <img src="https://raw.githubusercontent.com/iqp-samples/iqp-samples-integration-sqlserver/master/img/sql%20server%20settings%203.jpg" alt="adding new SQL Server connection">

    - Check the mappings in SQL destination editor. All inputs should been linked to proper output.
    <img src="https://github.com/iqp-samples/iqp-samples-integration-sqlserver/blob/master/img/sql%20server%20mappings.jpg?raw=true" alt="mappings">
    


- Now you can run project by clicking Start button on SSDT

## Results

- After script execution you can check that all step in data flow successfully complited

<img src="https://github.com/iqp-samples/iqp-samples-integration-sqlserver/blob/master/img/success%20run.jpg?raw=true" alt="SSDT success run">

- The result of project execution is a pivot table on SQL Server, which stores time presence each object in every zone in hours

<img src="https://github.com/iqp-samples/iqp-samples-integration-sqlserver/blob/master/img/sql%20server%20results.jpg?raw=true" alt="created table">