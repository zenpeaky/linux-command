
cron job everyday at 13.15 with dynamic file name creation
```bash
15 13 * * * pg_dump -h dbhost -U dbuser -p 5432 -d dbname > /drive/backup/`date "+\%Y-\%m-\%d"`_dbname.bak
```

crin job every saturday at 13.20
```bash
20 13 * * 6 cd /drive/backup && git add `date "+\%Y-\%m-\%d"`_dbname.bak && git commit -m "update db" && git push origin main
```
