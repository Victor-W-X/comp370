Task3:

* There are 36860 entries, using "wc -l ./data/clean\_dialog.csv"
* There are four labels: "title","writer","pony","dialog", using "head -n 1 ./data/clean\_dialog.csv" and they contain strings.
* There are 196 episodes (splitting the 2-3 parter episodes as their own episode), using "tail -n +2 ./data/clean\_dialog.csv | cut -d',' -f1 | sort -u | wc -l", the important command being sort -u to get only the unique ones.
* There are some entries that have multiple ponies speaking, so it could get difficult to count. I used "less ./data/clean\_dialog.csv" to just look around several lines.



