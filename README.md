# Morgan Thomas project portfolio

Here are some selected open source projects I have worked on. They are in two categories: demoable projects which I did by myself or as the project leader, and non-demoable library code which I did in collaboration with others in some cases.

## Demos

I have four demos to share with you. All of these are projects which I did by myself or which I led. Source code is available for each of them.

### Fairy Chess

This is a two-player online game which is like chess, except that the rules for piece movement are generated randomly (within certain defined parameters). This program is written in JavaScript using the MEAN stack (MongoDB, ExpressJS, Angular 1, and Node). I did this by myself.

**URL:** http://morgan-thomas-demos.net:3000/

**Video demo:** https://www.youtube.com/watch?v=fBlJpnxy0fs

**Source:** https://github.com/morganthomas/fairy-chess

### 2048

This is a program which plays the game of 2048 using an AI algorithm and lets you watch it in real time. I have never seen it lose (i.e., fail to reach the 2048 tile). This program is written in JavaScript using jQuery. I did this by myself.

**URL:** http://morgan-thomas-demos.net:3001/

**Source:** https://github.com/morganthomas/2048-js

### New Hampshire Bill Sign In Tool

This is a website which allows you to submit your positions on bill hearings to the State of New Hampshire. It uses Selenium brower automation to operate the State of New Hampshire website, providing a more streamlined user interface for doing this task. This program is written using [Shpadoinkle](https://shpadoinkle.org), the Haskell UI framework.

**URL:** http://testify-nh.org/

**Source:** https://github.com/morganthomas/testify

### Shpadoinklekasten

This is a note-taking app based on the Zettelkasten concept. It is not finished and it is a little rough around the edges. I wrote this as my first full application using [Shpadoinkle](http://shpadoinkle.org/), the Haskell UI framework. This app uses the MongoDB on the backend. I led this project with two other collaborators, who helped me for the purpose of learning Shpadoinkle.

**URL:** http://morgan-thomas-demos.net:8080/app

You can log into this demo with the username `demo` and the password `password`.

**Source:**
 * Server: https://github.com/morganthomas/Shpadoinklekasten-server
 * Client: https://github.com/morganthomas/Shpadoinklekasten-client
 * Library (shared between the server and the client): https://github.com/morganthomas/Shpadoinklekasten-client
 * Docker build: https://github.com/morganthomas/Shpadoinklekasten-docker

## Library Code

### Shpadoinkle

I am a major contributor to [Shpadoinkle](https://shpadoinkle.org/), the Haskell UI framework. I am responsible for the concept of Shpadoinkle continuations, which is how Shpadoinkle allows for concurrent event handlers interacting with view models without race conditions. I am also responsible for Shpadoinkle's mechanisms for streaming data, lazy loading tables, and lazily populated tables.

**Source:** https://gitlab.com/fresheyeball/Shpadoinkle

### servant-client-js

This is an alternative to [`servant-client`](https://github.com/haskell-servant/servant) for use in web browsers. Servant is a Haskell framework for building APIs. `servant-client` is a part of Servant which deals with automatically creating functions to call Servant APIs. `servant-client` supports being used in web browsers, but in this context it does not support streaming HTTP responses, because under the hood it uses `XMLHttpRequest`, which does not support streaming responses. Therefore I made `servant-client-js`, which uses the Fetch API under the hood and supports streaming HTTP responses. I did this by myself. This library is a dependency of Shpadoinkle.

**Source:** https://github.com/morganthomas/servant-client-js

### Compactable and Categorical Compactable

This is a Haskell abstraction which greatly generalizes `catMaybes`. Isaac Shapira is primarily responsible for this library, but I helped him to flesh out the concept. I am also responsible for generalizing the concept of Compactable from the category of Haskell types and functions to arbitrary Categories, in the Categorical Compactable library, which is still only a sketch. Perhaps we will unify these two libraries someday.

**Source:**
 * Compactable: https://gitlab.com/fresheyeball/Compactable
 * Categorical Compactable: https://github.com/morganthomas/categorical-compactable/blob/master/src/Control/Categorical/Compactable.hs
