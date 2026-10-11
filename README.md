# Kino, a design prototype

Kino is Beli for movies, with a friend network: rank films through quick head-to-heads, see how your taste matches your friends', and pick films together as a group.

This is the coded prototype of design **V.2.2**. Everything runs in your browser and nothing is saved; the people are invented. On a phone you get the iPhone layout; at 900px and wider, the web layout.

**Open it:** https://noahohstudio.github.io/kino-prototype/ (the web with a top bar instead of the rail: https://noahohstudio.github.io/kino-prototype/?nav=top)

## New since V.2.1

- **Kino opens with a splash:** the crowd's dots gather around yours, every time it opens.
- **Your account:** you at the bottom of the rail (or the gear on your profile) opens Profile, Your stats, Invites, Settings and Sign out. Your stats ends with your member stub.
- **Signing in and joining:** sign out, then "Not Dani?" to join. You can join taste first (tap what you've seen, a few quick choices, your top 3 appears) or from a friend's invite, where your taste match is the moment.
- **Ranking:** pick which film first, then a feeling, head-to-heads (or "Haven't seen it"), and Rank another when you're done.
- **Your films:** rankings by feeling, a diary of every watch, a watchlist and lists that look like piles.
- **People:** everyone has a profile now. Tap a face or a name to open it. Takes show up to two replies, and all of them in a sheet.
- **Every film has a page:** a backdrop, a trailer, your score, your friends' scores, and where to watch.
- **Waiting and when things go wrong:** colourful loading dots, what you saw last while Kino catches up, a slow-connection line, offline that keeps your vote waiting as a hollow dot, empty spaces that always offer something to start from, and errors that stay in place.
- **Asking first:** after your first vote in a group, Kino asks in its own words before iOS (or the browser) asks about notifications.

## Things to try

- Vote in Thursday film club, then say yes or Not now.
- Open any film from Home or Explore.
- On the web, pick up a pile on Explore.
- Sign out from your menu, then join as someone new.

## Notes for the developer

- **Sample data:** people, scores, takes, member numbers and where to watch are invented. Where to watch is sample data until a provider is wired in (for example TMDB's watch providers, which come from JustWatch).
- **Backdrops:** a film page shows a real still when we can match one to its film for certain. Otherwise it shows the poster's colour with a field of dots, in the same place, for the film library to fill in.
- **What iOS decides:** push notifications use iOS's communication style, led by the sender's photo. iOS puts the app's icon on the corner of that photo itself, and an app can't remove it. The prototype draws the intent: a cream dot, the same "new" marker as the bell.
- **What the browser decides:** on the web, the browser shows its own notification prompt, and there are no contacts to ask for.

Film posters and stills belong to their studios and appear here for a non-commercial design study.
