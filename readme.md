# LVMath

The internal website of the Lawrenceville Math Club.

# Development (Python 3.9)

## Notes

- Currently, when working with SQLAlchemy, use https://docs.sqlalchemy.org/en/14/tutorial/index.html.

## To Do

- Add `setup.py` for deployment.
- Connect SQLAlchemy Column.default and WTForms Field.default in `model_form`.

## Environment Setup

### macOS

```
python3 -m venv venv
source venv/bin/activate
python3 -m pip install -r requirements.txt
```

### Windows

```
py -m venv venv
venv\Scripts\activate
py -m pip install -r requirements.txt
```

## Format (Before Commit)

### macOS

```
python3 -m black .
```

### Windows

```
py -m black .
```

## Environment Variables

- The `DATABASE_URL` environment variable should point to the database (including SQL driver).
- The `sqlalchemy.url` variable in `alembic.ini` should be set to the value of `DATABASE_URL`.
