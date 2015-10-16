---
layout: post
title: MySQL import into Azure (ClearDB) via PowerShell
---

I attempted to import a MySQL database I had previously exported today via PowerShell, and was greeted with this lovely error:

![](https://raw.githubusercontent.com/daveyb/daveyb.github.io/master/images/mysql-ps-1.PNG)

For the record, the import command was:

```
mysql -h [hostname] -u [user] -p [tablename] < backup.sql
```

And the error thrown, "The '<' operator is reserved for future use.".

The fix is to read each line of the data into PowerShell as an object using Get-Content, then pipe it to MySQL... sort of the opposite of the method above, like so:

```
Get-Content .\backup.sql | mysql -h [hostname] -u [user] -p [tablename]
```

Hope this helps somebody else, or future me.
