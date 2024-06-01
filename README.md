## The DVDRental Postgres Sample DB

First, download the file and save it somewhere on your drive. It's a TAR file (an archive), and you'll use it directly when loading. Remember its location (you could save it in C:\dvdrental if you're on Windows).

To load this file, follow these steps:"

```
create dasbase dvdrental
```

This will create the sample DB. Then, you'll need to run pg_restore. If you're on windows this is in `C:\Program Files\PostgreSQL\16\bin` (make sure your version is correct).

If the bin is in your path, you should be able to run `pg_restor` straight away.

Now, run it:

```
pg_restore -U postgres -d dvdrental C:\dvdrental\dvdrental.tar
```

That's it - you should be good to go.
