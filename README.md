# Kino, a design prototype

Kino is Beli for movies, with a friend network: rank films through quick head-to-heads, see how your taste matches your friends', and pick films together as a group.

This is the coded prototype of design **V.2.2**. Everything runs in your browser and nothing is saved; the people are invented. On a phone you get the iPhone layout; at 900px and wider, the web layout.

**Open it:** https://noahohstudio.github.io/kino-prototype/ (the web with a top bar instead of the rail: https://noahohstudio.github.io/kino-prototype/?nav=top)

## Updated on October 11, 2026

- **A tighter web:** groups, the vote, It's settled., profiles and film pages now read like Home: a small, steady type scale, weight and grey for hierarchy, hairline rows instead of boxes, smaller thumbnails.
- **Opening things:** what you tap travels to its place on the next screen. A poster becomes the film page's poster, a face becomes the profile's, and a list's pile deals its films out.
- **Hovering on the web:** hover a poster to see which friends ranked it and their scores, in a card beside it.
- **Back online:** the offline line slips away and your waiting vote fills with a little pop. Try again on the line brings you back sooner.
- **Editing lists:** Edit fans every pile open, so you can see what's in them.
- **A few fun ones:** tap kino at the top of Home and the crowd gathers again; double-tap a friend's take to like it; a friend's match counts up on their profile; It's settled. bursts with the crowd's dots.
- **Smoother, later the same day:** opening a film or a profile no longer flashes (the old screen fades away while the poster travels); back online, the line folds away and everything moves up in one piece; long lists deal only what's on screen, and posters further down load as you reach them.
- **Who's voted:** the check on a voter's face sits just off its top right, like every other marker.
- **A more menu on takes** (the last piece from the original): on iPhone, press and hold a take (or tap its “…”) and it lifts, with the menu right under it; on the web, the “…” shows when you point at a take, and a right-click opens the same menu. Rank it, Save, Add to a list, Share, Hide this take (with Undo) and Report (a reason, then thanks).

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
- On the web, hover a poster on Home, Explore or My films.
- Double-tap what a friend said in your feed.
- Press and hold what a friend said in your feed, or right-click it on the web.

## Notes for the developer

- **Sample data:** people, scores, takes, member numbers and where to watch are invented. Where to watch is sample data until a provider is wired in (for example TMDB's watch providers, which come from JustWatch).
- **Backdrops:** a film page shows a real still when we can match one to its film for certain. Otherwise it shows the poster's colour with a field of dots, in the same place, for the film library to fill in.
- **What iOS decides:** push notifications use iOS's communication style, led by the sender's photo. iOS puts the app's icon on the corner of that photo itself, and an app can't remove it. The prototype draws the intent: a cream dot, the same "new" marker as the bell.
- **What the browser decides:** on the web, the browser shows its own notification prompt, and there are no contacts to ask for.
- **A take's menu:** it opens after a 0.52s hold, and moving more than 8px lets go (that's a scroll). Report is the design only: it needs a real moderation queue behind it.
- **Long lists:** only what's on screen animates (12 films at most), and posters past the first screenful load lazily. In the real build, virtualise long lists and page the feed in.
- **Motion:** two curves, Kino's ease (0.2, 0.7, 0.2, 1) and a small spring (0.3, 1.35, 0.5, 1); anything in your way stays under 0.6 seconds. Reduced motion turns it all off.

Film posters and stills belong to their studios and appear here for a non-commercial design study.
