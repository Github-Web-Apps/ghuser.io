The database is here to cache GitHub's data.

During the prototyping phrase, it's just a JSON file that we update once per day by running

```bash
$ npm install
$ ./fetch.js
```

To serve one more user, add an empty user to `db.json`:

```json
{
  "_comment": "DO NOT EDIT - Generated by ./fetch.js",
  "users": {
    "AurelienLourot": {
      "...": "..."
    }.
    "myNewUser": {}
  },
  "...": "..."
}
```

and run

```bash
$ ./fetch.js
```