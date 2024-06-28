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

Abteilungen 1 und 4 der Untersuchungsrichterregion 2 mit den Gebieten der Militärpolizeiposten Oensingen, Worblaufen, Thun, Sarnen und Goldau.

Abteilungen 2 und 3 der Untersuchungsrichterregion 2 mit den Gebieten der Militärpolizeiposten Brugg, Kloten, Oberuzwil, Mels und Thusis.
