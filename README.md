# NODE.JS - TypeScript Setup With Node & Express

### About

A quick and dirty way to get started with TypeScript and Node.js. We cover the basics of how to get started with TypeScript and  how to use TypeScript with the Node.js framework Express.

```
import express, { Application, Request, Response, NextFunction } from "express";

const app: Application = express();

const add = (a: number, b: number): number => a + b;

app.get("/", (req: Request, res: Response, next: NextFunction) => {
    console.log(add(1, 2));
  res.send("Hello World!");
});

app.listen(5000, () => console.log("Example app listening on port 5000!"));
```
