---
layout: post
title: Spring method security
---

Spring Security is ...

Spring Security can work at the method level, specifying who is allowed to access this method.

At its simplest, we can apply method security based on roles...

@
void updateAccount()

...

While this may be sufficient for many scenarios, it does not cover occassions where access to a method depends on the users relationship with a particular object in the system. Take the example of a bank account service where any known user is allowed to access a particular method:

void updateAccount(AccountDetails updatedDetails);

It makes sense that a User can access the updateAccount method, but they should only access it with the AccountDetails object that relates to their account.

...



[Jekyll](http://jekyllrb.com) is a static site generator, an open-source tool for creating simple yet powerful websites of all shapes and sizes. From [the project's readme](https://github.com/mojombo/jekyll/blob/master/README.markdown):

  > Jekyll is a simple, blog aware, static site generator. It takes a template directory [...] and spits out a complete, static website suitable for serving with Apache or your favorite web server. This is also the engine behind GitHub Pages, which you can use to host your project’s page or blog right here from GitHub.

It's an immensely useful tool and one we encourage you to use here with Hyde.

Find out more by [visiting the project on GitHub](https://github.com/mojombo/jekyll).