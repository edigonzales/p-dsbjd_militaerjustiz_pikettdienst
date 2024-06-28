# p-dsbjd_militaerjustiz_pikettdienst

```
docker compose run --rm -u $UID --workdir //home/gradle/schema-jobs/shared/schema \
  gretl -PtopicName=dsbjd_pikettregionen_militaerjustiz -PschemaDirName=schema createSchema configureSchema
```

```
docker compose run --rm -u $UID --workdir //home/gradle/schema-jobs/shared/schema \
  gretl -PtopicName=dsbjd_pikettregionen_militaerjustiz -PschemaDirName=schema dropSchema
```

```
java -jar /Users/stefan/apps/ili2pg-5.1.0/ili2pg-5.1.0.jar --dbhost localhost --dbport 54321 --dbdatabase edit --dbusr ddluser --dbpwd ddluser --disableValidation --models SO_DSBJD_Pikettregionen_Militaerjustiz_20240628 --dbschema dsbjd_pikettregionen_militaerjustiz_v1 --export fubar.xtf
```

```
java -jar /Users/stefan/apps/ilivalidator-1.14.2/ilivalidator-1.14.2.jar fubar.xtf
```



```
docker compose run --rm -u $UID --workdir //home/gradle/schema-jobs/shared/schema \
  gretl -PtopicName=dsbjd_pikettregionen_militaerjustiz -PschemaDirName=schema_pub createSchema configureSchema
```

```
docker compose run --rm -u $UID --workdir //home/gradle/schema-jobs/shared/schema \
  gretl -PtopicName=dsbjd_pikettregionen_militaerjustiz -PschemaDirName=schema_pub dropSchema
```

```
docker compose run --rm -u $UID gretl --project-dir=dsbjd_ausgleichsabgabe_pub
```


ch.swisstopo.pixelkarte-farbe

swisstopo erstellt Landeskarten in den Massstäben 1:10`000 bis 1:1 Million. Der Layer Landeskarten (farbig) nutzt die unterschiedlichen Massstäbe und zeigt die geeignetste Karte in Abhängigkeit der gewählten Zoomstufe an. Der Layer Landeskarte (farbig) dient als Hintergrundkarte im Geoportal des Bundes. Er ist auch in den Geodiensten WMS und WMTS verfügbar.