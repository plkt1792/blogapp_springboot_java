# Blogging App


## JSON Entities

### User
```
{
	"id"		: "411",
	"username"	: "omshiv",
	"email"		: "shivoham@blog.com",
	"password"	: "XXXXXXXXX",
	"authToken"	: "jfnkdsajfhl132#*&r1kebdaksdn@%Rakn121$kajbd"
	"bio"		: "nothing and everything",
	"image"		: "https://imgur.com/shiv.png"
}
```
### Profile
```
{
	"username"	: "omshiv",
	"bio"		: "nothing and everything",
	"image"		: "https://imgur.com/shiv.png"
}
```

### Article
```
{
	"id"		: 75213,
	"title"		: "End and Begining of Everything",
	"slug"		: "end-and-begining-of-everything",
	"subtitle"	: "The pathway from ego to enlightenment",
	"bio"		: "This is an article about.... <b>Ego</b> and path to <b>Enlightenment</b>....",
	"createdAt"	: "2023-01-01 03:45:00"
}
```

### Comments
```
{
	"id"		: 23112
	"title"		: "Mind blow",
	"subtitle"	: "I found purpose of life",
	"createdAt"	: "2023-01-01 03:45:00"
}
```

## API Endpoints

### Create a new user
### `POST /users` 
---
### User login
### `POST /users/login` 
---
### Get profiles of all the users 📄
### `GET /profiles` 
---
### Get details of a particular user
### `GET /profiles/{username}` 
---
### Get all articles 📄
### `GET /articles`
**Default page size = 10**

**Available Filters:**
- `/articles?tag=stocks`
- `/articles?author=omshiv`
- `/articles?page=3&size=10`
---
### Get an article
### `GET /articles/{article-slug}`
---
### Create a new article 🔐
### `POST /articles`

---
### Edit an article 🔐 👤
### `PATCH /articles/{article-slug}`
---
### Get all comments of article 📄 
### `GET /articles/{article-slug}/comments`
---
### Post a comment on an article 🔐
### `POST /articles/{article-slug}/comments` 
---
### Delete comment of an article 🔐 👤
### `DELETE /articles/{article-slug}/comments/{comment-id}` 
---

## Schema Design
Checkout [Entity Relational Diagram](http://tinyurl.com/mrf28e7z)
