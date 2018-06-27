# tito-http   
[![Build Status](https://travis-ci.org/adityamedhe/tito-http.svg?branch=master)](https://travis-ci.org/adityamedhe/tito-http)
---
A well documented HTTP Server implementation in NodeJS using TypeScript meant for those who want to learn and experiment with HTTP

## What is HTTP?
I doubt anyone will need this answer, but for the sake of completeness, here you go: https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol

## Why are you building an HTTP/1.1 Server from scratch?
Good question. There are several HTTP Server implementations viz. nginx, Apache, and Node's `http` that are faster, efficient, and scalable than `tito-http` will ever be. However the goal is not to compete with them on performance or efficiency. Infact the goal is not even to become a commercially used HTTP server. 
As they say, you must know your tools inside out, and I am not a fan of having superficial knowledge atleast on things I use daily, I decided to craft a HTTP server on my own, and also make it available to others so that they can look at the code and understand how it looks like. The main goal of this project is learning, both for you and me. If this project is successful and widely-known, I would prefer it to be known as a good starting point and reference for learning HTTP in depth, rather than something which wants your attention to be used in production in your next project. Nah. Many smart(er) people have already achieved that in a much, much better way than this project will probably ever be able to.

## What are you refering to, as the HTTP standard?
I initially started out with RFC 2616. However that seemed too dry a document to base my learning on, and anyway it's obsolete now, hence this project will be based on the learning from the following resources.

- For basic introduction and getting your feet wet, read the Wikipedia article or any other "introduction to HTTP" from a credible source.
- Next, we refer to [HTTP Overview](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview) and [Basics of HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP) articles on MDN.
- For settling all disputes, or looking for some obscure information that the above docs don't cover, the final authority is the RFC 723x family of RFCs, which obsoleted RFC2616 in 2014. Mainly, two RFCs are of interest:
   - [RFC7230](http://tools.ietf.org/html/rfc7230): HTTP/1.1 Message Syntax and Routing
   - [RFC7231](http://tools.ietf.org/html/rfc7231): HTTP/1.1 Semantics and Content

## What is the language/platform of choice?
It's NodeJS + TypeScript.
- NodeJS: Because that's the framework I work with daily and know a thing or two about, and I don't want to learn a new language/framework solely for this. Besides, it offers a good TCP implementation to base our HTTP server on, via its `net` module.
- TypeScript: Because why not! Since the primary objective of this project is learning, it makes all the more sense to go with a typed language. Think all the types we can annotate HTTP Requests/Responses and internal data with! Once complete the code should read like a story with all the types and docs.

## Why the name `tito-http`?
"Tito" was the monicker of my four legged friend, a dark golden labrador retriever, whose company I enjoyed for 11 years from 2005-2016. The project is named after recognizing the similarity of the characteristics of HTTP and his presence in my life: indispensable and omnipresent.