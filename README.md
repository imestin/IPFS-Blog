# IPFS-Blog
Decentralized blog based on IPFS. Can be used as a news site. Experimental.

__NOTE__: this is just a repository that contains the _ipfs-blog-daemon_, _ipfs-blog-uploader_ and _ipfs-blog-website_ in one repository.

## Live version

Live version: https://ipfs.io/ipns/k2k4r8l53zrytcl9ka78eh5890syyg9jh543m08k4g60isrgljd462r1/
(magyar) Ez ennek a weboldalnak a forráskódja:
https://ipfs.io/ipns/k2k4r8nsj5rscg5xkkelcjhgtapmm6s8xvz9biragt9ejfchca3qcy4f/

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


__UPDATE__: Current version does not use OrbitDB, it uses only IPFS, the database is a json file.
