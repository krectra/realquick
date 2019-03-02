#### Cleaning pyc files
```bash
$ find . -name "*.pyc" -exec rm -f {} \;
```



## QGIS
#### Icon
Upon changing an icon, do a compile to apply changes:
```bash
$ make
```


## Django
#### Migrations
Reverting from a specific migration version
```bash
$ python manage.py migrate <app_name> 0002_previous_migration
```

Reverting before initial
Example:
```bash
$ python manage.py migrate <app_name> zero
```

#### ERD
Generate ERD image
Install `django-extensions`, `graphviz` and `pydotplus` packages then
```bash
$ python manage.py graph_models -a -g -o model.png
```
