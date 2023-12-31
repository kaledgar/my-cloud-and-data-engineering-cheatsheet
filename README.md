# my-cloud-and-data-engineering-cheatsheet
My cloud/ data engineering/ devops / dev eveything cheatsheet.

## SQL 

Count rows in table

```SQL
SELECT COUNT(*) FROM table
```

Best Query to test connection

```SQL
-- oracle
SELECT 1 FROM DUAL

-- MySql / Redshift
SELECT 1
```

## Formatting SQL

SQLfluff is great for formatting SQL

```bash
# installation
pip install sqlfluff

# check version
sqlfluff version
which sqlfluff
```

Formatting

```bash
sqlfuff lint "filepath.sql"
sqlfuff parse "filepath.sql"
sqlfuff fix "filepath.sql"
```

## VSC settings

```json
{
    "python.defaultInterpreterPath": "/usr/bin/python3",
    "python.testing.pytestEnabled": true,
    "python.testing.unittestEnabled": false,
    "python.testing.pytestArgs": [
        "."
    ],
    "python.envFile": "${workspaceFolder}/.env",
    "python.linting.enabled": true,
    "python.linting.pylintEnabled": true,
    "editor.fontSize": 15,
    "editor.formatOnSave": true,
    "[python]": {
        "editor.formatOnType": true,
        "editor.defaultFormatter": "ms-python.black-formatter"
    },
    "sqlfluff.config": ".sqlfluff",
    "sqlfluff.executablePath": "sqlfluff_path"
}
```

