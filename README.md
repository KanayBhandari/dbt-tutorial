# dbt-tutorial
This is a learning repository for DBT

### Quickstart for dbt Core from a manual install
https://docs.getdbt.com/guides/manual-install?step=1


Setup:

1. Create virtual env using command
`python -m venv dbt-env`

2. Activate the virtual env
`source dbt-env/Scripts/activate`

3. Install the required adapter(in my case I want to connect to postgres adapter)
`python -m pip install dbt-postgres`

4. Follow the quickstart guide for dbt core:
`https://docs.getdbt.com/guides/manual-install?step=1`

5. In your database create two table manually to do the hands on:
```
CREATE TABLE dbt_kanay.customers (
    id SERIAL PRIMARY KEY,
    first_name VARCHAR(50),
    last_name VARCHAR(50)
);

CREATE TABLE dbt_kanay.orders (
    id SERIAL PRIMARY KEY,
    user_id INT,
    order_date DATE,
    status VARCHAR(50)
);
```
