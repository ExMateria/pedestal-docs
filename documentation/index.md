<!--
 Copyright 2013 Relevance, Inc.

 The use and distribution terms for this software are covered by the
 Eclipse Public License 1.0 (http://opensource.org/licenses/eclipse-1.0)
 which can be found in the file epl-v10.html at the root of this distribution.

 By using this software in any fashion, you are agreeing to be bound by
 the terms of this license.

 You must not remove this notice, or any other, from this software.
-->
---
title: Pedestal Documentation
---

## What is Pedestal?

Pedestal is a collection of
interacting libraries that together create a pathway for developing
a specific kind of application. It empowers developers to use
Clojure to build internet applications requiring real-time
collaboration and targeting multiple platforms.

In short: Pedestal provides a better, cohesive way to build
rich client web applications in Clojure.

## Who is it for?

Clojurists looking for a standard way to build internet
applications will love Pedestal. Rather than composing art
out of found objects, they will now be able to mold a single,
consistent form to match their vision.

Pedestal may also appeal to developers who have been nervously
approaching a functional language but who haven't yet mustered the
courage to ask it out on a date. It provides a sterling example
of how to use the Clojure ecosystem to its best advantage, reducing
the friction usually associated with a language switch.

## Where do I start?

In the _Getting Started_ section, you will find a walk-through
that introduces you to all of Pedestal's moving parts via the
creation of a new application. It explains the features
you'll find in the `pedestal.app` namespace.

_App Docs_ covers higher-level topics, and pulls back the
curtain on the reasoning behind Pedestal's approach.

_Service Docs_ gets down and dirty with the inner workings of
the `pedestal.service` layer.

## What about API Documentation?

To generate literate-programming-style documentation for the `app` and
`service` libraries, add the [lein plugin for
marginalia](https://github.com/fogus/lein-marginalia) to your lein user
profile. After installing the pedestal libraries you can then `cd` into the
`app` or `service` directories and run `lein marg`.

```bash
cat ~/.lein/profiles.clj
# {:user {:plugins [[lein-marginalia "0.7.1"]]}}

git clone https://github.com/pedestal/pedestal.git
cd pedestal
lein sub install
( cd app && lein marg )
( cd service && lein marg )
```

This will create the documentation for `pedestal.app` and
`pedestal.service` in their respective `docs` directory.
