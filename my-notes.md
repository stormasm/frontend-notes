
So everything is intact from
[spec-md](https://github.com/leebyron/spec-md)
and all I did was add a command to build my own personal blog / spec.

Initially out of the box when you run

```
npm install
```

the original spec-md spec gets built...
Then if you want to modify or change your frontend-notes simply run the command

```
npm run go
```

whose **go** tag is documented in package.json explaining exactly what it does.

It overwrites the spec-md with your blog and then you can push the changes in
the out directory into the branch gh-pages.
