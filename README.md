# migration-oracle-iris
Sample repository to show how to migrate from Oracle to InterSystems IRIS

# Credits
1. Article about Oracle into Docker: 
    - https://hub.docker.com/r/gvenzl/oracle-xe
2. Git project created from: 
    - https://github.com/intersystems-community/iris-docker-zpm-usage-template

# to run
1. Build
```
docker-compose build
```
2. Run
```
docker-compose up -d
```
3. Use DBeaver to connect to the databases
    - **Connection to Oracle**: 
        - host: localhost 
        - database: XE 
        - port: 15210 
        - username: sys 
        - password: Welcome1
    - **Connection to IRIS**: 
        - host: localhost 
        - database: user 
        - port: 1972 
        - username: _SYSTEM 
        - password: SYS

4. Go to SAMPLEDB schema to access data loaded from the script init_scripts/sampledb.sql