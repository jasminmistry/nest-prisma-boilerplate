## NestJs Prisma Boilerplate

## Installation

```bash
$ npm install
```

```bash
$ npx prisma migrate dev --name init
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

URLs:

GET

/post/:id: Fetch a single post by its id
/feed: Fetch all published posts
/filter-posts/:searchString: Filter posts by title or content

POST
/post: Create a new post
Body:
  title: String (required): The title of the post
  content: String (optional): The content of the post
  authorEmail: String (required): The email of the user that creates the post
/user:x Create a new user
Body:
email: String (required): The email address of the user
name: String (optional): The name of the user

PUT
/publish/:id: Publish a post by its id

DELETE
/post/:id: Delete a post by its id
