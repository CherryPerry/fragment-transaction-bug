### Description

If activity stops while fragment transition is running,
both of fragments are drawn after start,
but the old one does not exist, just drawn like a ghost.

### Steps to reproduce
1. Add fragments to backstack with `setTransition(FragmentTransaction.TRANSIT_FRAGMENT_FADE)`
1. Call `onBackPressed()` and click recent apps at the same time.
1. Open app from recent list
1. Both of fragments are drawn, but clickable only valid one

### Video

![ezgif-2-cf08197654](https://user-images.githubusercontent.com/9081555/43469630-48f3759e-94ef-11e8-825b-5b18c92bf1c1.gif)
