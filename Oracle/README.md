# Netkiller Oracle templates

## Create monitor user

CREATE USER ZABBIX
IDENTIFIED BY <REPLACE WITH PASSWORD>
DEFAULT TABLESPACE USERS
TEMPORARY TABLESPACE TEMP
PROFILE DEFAULT
ACCOUNT UNLOCK;
GRANT ALTER SESSION TO ZABBIX;
GRANT CREATE SESSION TO ZABBIX;
GRANT CONNECT TO ZABBIX;
ALTER USER ZABBIX DEFAULT ROLE ALL;
GRANT SELECT ON V_$INSTANCE TO ZABBIX;
GRANT SELECT ON DBA_USERS TO ZABBIX;
GRANT SELECT ON V_$LOG_HISTORY TO ZABBIX;
GRANT SELECT ON V_$PARAMETER TO ZABBIX;
GRANT SELECT ON SYS.DBA_AUDIT_SESSION TO ZABBIX;
GRANT SELECT ON V_$LOCK TO ZABBIX;
GRANT SELECT ON DBA_REGISTRY TO ZABBIX;
GRANT SELECT ON V_$LIBRARYCACHE TO ZABBIX;
GRANT SELECT ON V_$SYSSTAT TO ZABBIX;
GRANT SELECT ON V_$PARAMETER TO ZABBIX;
GRANT SELECT ON V_$LATCH TO ZABBIX;
GRANT SELECT ON V_$PGASTAT TO ZABBIX;
GRANT SELECT ON V_$SGASTAT TO ZABBIX;
GRANT SELECT ON V_$LIBRARYCACHE TO ZABBIX;
GRANT SELECT ON V_$PROCESS TO ZABBIX;
GRANT SELECT ON DBA_DATA_FILES TO ZABBIX;
GRANT SELECT ON DBA_TEMP_FILES TO ZABBIX;
GRANT SELECT ON DBA_FREE_SPACE TO ZABBIX;
GRANT SELECT ON V_$SYSTEM_EVENT TO ZABBIX;
