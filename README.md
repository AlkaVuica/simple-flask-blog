# simple-flask-blog
This is a simple RESTful blog website built with Flask using Python.

The first registered user is considered admin and can **publish** and **edit** posts on the website. Other users can register to comment on the blog posts.

---

The blog uses **SQLite** as database for local development, but if deployed for production, database should be switched to **PostgreSQL**.
```
# CONNECT TO DB
app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite:///blog.db'
```
should be changed to
```
# CONNECT TO DB
app.config['SQLALCHEMY_DATABASE_URI'] = 'postgres:///(YOUR DB URI)'
```
