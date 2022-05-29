# whiteboard-interview-prep-guide
Resource for preparing for a technical coding interview

# Systems Design
## Databases
- how transactions work
- types of databases
  - SQL/relational
  - NoSQL
    - key-value (redis)
    - wide column (Cassandra)
    - Document (MongoDB)
- ACID vs BASE
- horizontal scaling
  - CAP Theorem
  - sharding via partitioning functions and pros/cons of each
    - hash, list, and range partitioning
  - read/write replicas
    - pro-tip: if the interviewer implies or explicitly states that most transactions are read-only, a read-only database replica is a great first answer

## Web Services
- when to use caching (usually via memcached) in place of a DB transaction
  - how would you design caching to reduce load on the database? Hint: what common queries can you group together to cache
- when to use a job/task queue on the backend
- What load balancers are and why web services use them
  - load balancing techniques https://kemptechnologies.com/load-balancer/load-balancing-algorithms-techniques/

Practice problems
- If you were to build Instagram with its most basic features (posting, liking, commenting, activity feed, and messaging other users), how would you design a system to serve this application?
- Load Balancer
- Load Balancing Algorithms and Techniques
- How does a load balancer distribute client traffic across servers?


In a systems design interview, your interviewer will want you to demonstrate general knowledge of how to design a system given a scenario or example. As you walk through your design, expect them to ask you to dive into a particular part of the system and ask you to identify potential bottlenecks and describe scaling techniques for that particular part of the system. What you are asked to go into detail about is up to the interviewer. You should have a good understanding of how to scale every part of the system you designed. If you do not know how to scale a part of your system, do not implement that part of the system. Which means that for the essential parts of a system that you cannot leave out, particularly load balancers and databases, you should develop a deep understanding of how they are implemented and how to scale them. You should always start with the most basic design with respect to the prompt, and only add to your system when necessary (just like in the real world).



# Resources

## Big-O
- https://bigocheatsheet.io/


## Good leetcode problems
https://neetcode.io/

https://www.techinterviewhandbook.org/grind75

### list (may contain duplicates)
- https://leetcode.com/problems/reverse-string/
- https://leetcode.com/problems/missing-number/
- https://leetcode.com/problems/valid-palindrome/
- https://leetcode.com/problems/number-of-good-pairs/
- https://leetcode.com/problems/kids-with-the-greatest-number-of-candies/
- https://leetcode.com/problems/unique-number-of-occurrences/
- https://leetcode.com/problems/height-checker/
- https://leetcode.com/problems/running-sum-of-1d-array/
- https://leetcode.com/problems/number-of-islands/
- https://leetcode.com/problems/longest-common-prefix/
- https://leetcode.com/problems/roman-to-integer/
- https://leetcode.com/problems/two-sum/