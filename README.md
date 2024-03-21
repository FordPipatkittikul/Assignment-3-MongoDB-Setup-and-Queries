# Assignment-3-MongoDB-Setup-and-Queries

## question 1

**query** : db.movies.find({year: 1983, runtime: {$gt: 200}}).sort({ runtime: 1}).projection({_id: 0,runtime: 1, title:1, year:1})

![Screenshot (73)](https://github.com/FordPipatkittikul/Assignment-3-MongoDB-Setup-and-Queries/assets/121902625/a2fcf39a-7349-415f-8daf-b271b97ead6f)

## question 2
**query** : db.movies.find({year: { $gt: 2014 },"imdb.rating": { $gt: 9 }}).sort({ "imdb.rating": -1 }).projection({ _id: 0, title: 1, year: 1, "imdb.rating": 1 })
