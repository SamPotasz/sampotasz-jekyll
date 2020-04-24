---
title: Subscriptions in React and Phaser.io
date: 2020-04-21 00:00:00
published: false
description: 
# featured_image: '/images/demo.jpg'
---

Observable: wrapping around the stream of events to do something with the data

Observer: 
    next: (nextValue) =>
    error: (error) =>
    complete () =>

Subscriptions tie observers to observables via a listener.

In gamedev, we usually only have one function on a listener.

In frontend dev, we want to supply three functions to the observable: next, error, and complete. (except we usually skip complete because the stream is always open)

And we're used to unsubscribing when things shut down so we don't have memory leaks. 

In React, we unsubscribe in componentWillUnmount.

---

Redux-thunk

Start, success, failure pattern. Moving isLoading/isFetching state storing onto redux. Which is nice.

Middleware - catches all actions with dispatch that *aren't* objects. Only cares about functions.

