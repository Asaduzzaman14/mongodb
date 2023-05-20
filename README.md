# mongodb
 ## find user by email
```
db.practis.find({email:"emilyroberts@example.com"})
```

### Find all users over 30 whose favorite color is "purple".
```
db.practis.find({
        age: { $gt: 30 },
        "favorites.color": "purple"
    })
 ```
 
 ### Find all users with "pizza" as their favorite food and sort them according to age.
 ```
 db.practis.find({
    "favorites.food": "pizza"
}).sort({ age: -1 })  // or age: 1
 ```
