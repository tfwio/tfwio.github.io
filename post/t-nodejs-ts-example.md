---
title: "NodeJS Typescript Blog Example (feat static export)"
date: "2021-01-01"
tags: [
  "node-ts-blog"
]
---

So am using a particular nextjs example upgraded to Typescript
with a few select added things.

Generally we just follow the provided NextJS tutorial on converting
a provided example into a Typesript project.

All the following steps are taken from the tutorial.


> note: This is really easy getting to work with Typescript, though
  "out of the box" it doesn't play nicely with Material-UI.

1. **Download Starter Code**
  ```bash
  npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn-starter/tree/master/basics-final"
  ```

2. **Create tsconfig.json**  
  Yeah.  this easy.  Its generated in our next step when you call on node or yarn.
  ```bash
  touch tsconfig.json
  ```

3. **Rename** all the \***.js** files \***.tsx**.

4. **OPTIONAL PART APPLIED TO THIS SOURCE CODE REPOSITORY**  
   Now what I did at this point is move things like moving all the directories: components, lib and styles
   into a new `./sources` directory and make sure everything refactored nicely.

   As long as ***your*** happy is all that matters.  If you clone this repository, you're getting
   the `./sources` directory, otherwise following the steps described here this is abbsolutely optional.

5. **Clean up whatever breaks EXPORTing**  
  Luckily the starter just uses `next/image` or a custom **Image** *Component* and all I had to do was find the two
  of them and convert them into standard images in order to provide working exports.  
  Using your IDE or editor (Visual Studio Code or what-not) find the 'Image' tags as used in layout.ts

  If you don't fix the images, **next EXPORT** fails.

6. At this point we can just call **Yarn** or **NPM** from the (git root) or working directory.
  ```bash
  yarn
  -- or --
  npx
  ```


<!-- https://www.astrotheme.com/ -->

A little more information about our configuration
-------------------------------------------------

- [Remark](https://github.com/gnab/remark/wiki) is used to provide Markdown to our NextJS/Typescript cofig here.
    - [gray-matter]
- [material-ui.com]










[gray-matter]:https://github.com/jonschlinkert/gray-matter
[material-ui.com]:https://material-ui.com/
