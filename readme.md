# Node containers

A few basic NodeJS containers. The base/latest image performs similarly to the
ONBUILD upstream version but reusable across projects. The brunch container
ensures that bower and brunch are installed.

We use these images to transpile and aggregate our frontend applications, then
serve them using an nginx container.

## Docker Compose example

```
app:
  image: c4tech/node
  volumes:
    - ./:/app
```
