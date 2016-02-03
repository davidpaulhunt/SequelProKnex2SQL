# SequelProKnex2SQL

Write queries using the KnexJS query builder and have it translated into pure SQL.

## Installation

Move the bundle into your bundles directory

```mv Knex2SQL.spBundle ~/Library/Application Support/Sequel Pro/Bundles/```

Reload your Sequel Pro bundles

```Bundles > Reload Bundles```

## Example Usage
In the query editor:
```js
knex('users').select('email').where('confirmed', false);
```
Press `ctrl + k`
and it becomes:
```sql
select `email` from `users` where `confirmed` = false
```
