# IPFS-Blog
Decentralized blog based on IPFS. Can be used as a news site. Experimental.

## Synopsis

We will use OrbitDB as a database. There will be 2 tables: a _users_ table and a _content_ table. In the content talbe, there will be _posts_, A post can contain text and images. Everything is encapsulated in JSON-compatible object.

First, the _content_ db will be implemented, creating new users will come second. In the first implementation, the admin will be the only users.

### Roles:
 * admin: can create new users
 * author: can create posts
 * reader: can read posts. Does not need to register to read posts. reader account registration won't be possible in the first version

 The idea that there will be IPFS seed servers, that will form a cluster. All nodes will host the full database. We want to create 2 tutorials, one for tech savvy people and one for non-tech savvy people.

 The more-complex tutorial will contain information about how to install an IPFS server, on a VPS.
 The less-complex tutorial will show how to install IPFS on a desktop computer or a phone, and pin the database of IPFS-Blog.

 It would be desirable to decentralize upload as well, but it's possible that first only access to the data will be decentralized.