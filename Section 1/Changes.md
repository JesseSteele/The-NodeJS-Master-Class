# Changes

## NEW: Changes for 2024

This document was last revised on March 1st, 2024

This course was originally released in 2018. Since then, the Node.js platform and ecosystem has continued to evolve. Here are the important changes that have happened since then, that you should be aware of:


### New version of Node:

The current stable version of Node (as of March 2024) is 20.11.1. That's the one you should be downloading and using.

You can download it here: [https://nodejs.org/en/]
You can read the docs here: [https://nodejs.org/docs/latest-v20.x/api/index.html]


### Use fs.ftruncate instead of fs.truncate

In newer versions of Node the name of the function used for file truncation has changed. As you watch the videos you'll see us refer to fs.truncate. You should be use fs.ftruncate instead (notice the exta "f" in the function name). You can see examples of how to use it here:

[https://nodejs.org/docs/latest-v14.x/api/fs.html#fs_fs_ftruncate_fd_len_callback]


### Node now has better support for ES6+

Newer node systems have better support for ES6 and beyond. The code presented in this course is ES5. If you use a newer version of Node we'd recommend using promises or async/await instead of getting into "callback hell". If you'd like to learn how to change ES5 syntax into ES6 , then check out our "Keeping up with the Javascripts" course. If you'd rather stick is ES5 that's fine as well. If you use ES6+ then you need to be careful about how you use the "import" syntax (in place of "require").  It's still tricky. Read this...

[https://nodejs.org/api/esm.html]

...and take careful note of these caveats:

[https://nodejs.org/docs/latest-v14.x/api/esm.html#esm_differences_between_es_modules_and_commonjs]


### Sorry, still no TypeScript support

Node still does not natively support TypeScript. If you want to use TS (which we don't actually recommend), you'll need to use a transpiler or a build system with this package. Again, we don't like this approach because we think it's already hard enough to debug Node's cryptic error messages without also having to figure out which line number in the error message equates to which line number in the original TS files. After you get super-comfortable with Node and have experience debugging it, then you could consider using TS without issues. But if you're just getting started, then using TS is setting yourself up for a world of pain.


### New Experimental Modules

The end of this course dives into bleeding-edge / experimental modules in Node. These are changing constantly. To see the latest experimental modules in the next version of node check out these docs here:

[https://nodejs.org/docs/latest/api/]


### This class has some bonus lectures

You'll see the details on the next slide in this course.

### Less Technical News

In less technical news, here are some interesting updates about the Node world. As you watch the lecture on "The Story of Node.js", you should keep these developments in mind as an addendum:

1. The Node.js project has moved yet again. Their new home is The Open JS foundation: [https://openjsf.org/]

2. Ryan Dahl (the author of Node) started a new project called Deno. It's arguably a Node.js competitor, and is built in Rust. Who knows what the future will bring. Will the projects merge together like Node did with io.js, or will they stay separate? We'll see. Find more here: [https://deno.land] and here: [https://github.com/denoland/deno] and read this too: [https://thenewstack.io/how-node-js-is-addressing-the-challenge-of-ryan-dahls-deno/]

3. NPM was sold to Github, which itself previously sold to Microsoft. So now Microsoft is technically the parent of Github and Github is the parent of NPM. More details here: [https://www.cnbc.com/2020/03/16/microsoft-github-agrees-to-buy-code-distribution-start-up-npm.html]