```sql
SELECT
    event,
    move,
    sum(nb_reps) as nb_reps
    from personal_bests
where event = 'SWCC#3'
group by event, move;
```


```sql
SELECT
    event,
    sum(nb_reps) as nb_total_reps
    from personal_bests
where event = 'SWCC#3'
group by event;
```

```sql
SELECT event,
    instagram_handle,
    nb_reps
from
    personal_bests
where
    move = 'MUSCLE_UP'
order by nb_reps desc limit 5;
```

```sql
SELECT event,
    instagram_handle,
    nb_reps
from
    personal_bests
where
    move = 'PUSH_UP'
order by nb_reps desc limit 5;
```


```sql
SELECT
    event,
    instagram_handle as athlete,
    sum(nb_reps) as nb_reps
    from personal_bests
where event = 'SWCC#3'
group by event, athlete
order by nb_reps desc;
```
