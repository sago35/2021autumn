---
key: two-phase-commit
title: The use of goroutines and channels in the example of two-phase commit
id: two-phase-commit
format: conference
talkType: ""
allroom: false
speakers:
- kojiaomatsu
---
Through actual examples of the use of goroutines and channels that I have encountered through my work, I will consider their general use.

To reduce the load on CloudSQL, we migrated some huge data to Datastore.
I will show the implementation of two-phase commit in the go language that I did.

---

Through actual examples of the use of goroutines and channels that I have encountered through my work, I will consider their general use.
To reduce the load on CloudSQL, we migrated some huge data to Datastore.
I will show the implementation of two-phase commit in the go language that I did.

Although I was impressed with the concurrency of the Go language, I never had a chance to actually use it.
I will explain why I needed it in the real world, what trade-offs I had to make, and how I implemented it.
