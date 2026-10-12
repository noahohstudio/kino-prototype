# Kino, a design prototype

Kino is Beli for movies, with a friend network: rank films through quick head-to-heads, see how your taste matches your friends', and pick films together as a group.

This is the coded prototype of design **V.2.3**, ready for review. Everything runs in your browser and nothing is saved; the people are invented. On a phone you get the iPhone layout; at 900px and wider, the web layout.

**Open it:** https://noahohstudio.github.io/kino-prototype/ (the web with a top bar instead of the rail: https://noahohstudio.github.io/kino-prototype/?nav=top)

## How to review

1. **Open it on your phone and on a laptop.** On iPhone, Safari's Share → Add to Home Screen gives the full-screen app. Kino opens with a short splash, then Home.
2. **Screens worth opening** (each link goes straight there):
   - Home: https://noahohstudio.github.io/kino-prototype/#/home
   - Explore, the piles: https://noahohstudio.github.io/kino-prototype/#/explore
   - A film: https://noahohstudio.github.io/kino-prototype/#/film/interstellar
   - A group's vote: https://noahohstudio.github.io/kino-prototype/#/group/thursday
   - A friend: https://noahohstudio.github.io/kino-prototype/#/profile/maya
   - You: https://noahohstudio.github.io/kino-prototype/#/me
   - Notifications: https://noahohstudio.github.io/kino-prototype/#/notifications
3. **Things to try:**
   - Vote in Thursday film club, say yes or Not now when Kino asks, then lock the pick: It's settled.
   - Tap a poster: it travels to the film's page. Tap a face to open a profile.
   - Rank a film (the + in the tab bar, or Rank a film on the web): a feeling, then quick head-to-heads.
   - Press and hold what a friend said in your feed (on the web, point at it for the "…", or right-click).
   - Double-tap a friend's take to like it. Tap kino at the top of Home.
   - On the web, hover a poster; pick up a pile on Explore.
   - Sign out from your menu (you, at the bottom of the rail, or the gear on your profile), then join as someone new.
4. **Worth knowing:** the people, scores, takes and where-to-watch are sample data. Report shows the design only (it needs a moderation queue). Real posters and streaming services need a data provider.

## What's new in V.2.3

- **A tighter web:** groups, the vote, It's settled., profiles and film pages read like Home: a small, steady type scale, weight and grey for hierarchy, hairline rows instead of boxes, smaller thumbnails.
- **Opening things:** what you tap travels to its place on the next screen. A poster becomes the film page's poster, a face becomes the profile's, and a list's pile deals its films out. The old screen fades away on top, so nothing flashes.
- **Hovering on the web:** a card beside a poster (never on it) shows which friends ranked it and their scores.
- **Back online:** the offline line folds away, everything moves up in one piece, and your waiting vote fills with a little pop.
- **Lists:** Edit fans every pile open; long lists deal only what's on screen, and posters further down load as you reach them.
- **A more menu on takes** (the last piece from the original): hold a take on iPhone and it lifts with its menu; on the web, the "…" shows when you point at a take, and a right-click opens it. Rank it, Save, Add to a list, Share, Hide this take (with Undo) and Report.
- **A few fun ones:** tap kino and the crowd gathers again; double-tap a take to like it; a friend's match counts up on their profile; It's settled. bursts with the crowd's dots.
- **Who's voted:** the check on a voter's face sits just off its top right, like every other marker.

## Earlier, in V.2.2

- **Kino opens with a splash:** the crowd's dots gather around yours, every time it opens.
- **Your account:** you at the bottom of the rail (or the gear on your profile) opens Profile, Your stats, Invites, Settings and Sign out.
- **Signing in and joining:** taste first, or from a friend's invite, where your taste match is the moment.
- **Ranking:** pick which film, then a feeling, head-to-heads (or "Haven't seen it"), and Rank another.
- **Your films:** rankings by feeling, a diary, a watchlist and lists that look like piles.
- **People:** everyone has a profile; takes show their replies.
- **Every film has a page:** a backdrop, a trailer, your score, your friends' scores, and where to watch.
- **Waiting and when things go wrong:** colourful loading dots, a slow-connection line, offline that keeps your vote waiting as a hollow dot, empty spaces with something to start from, and errors that stay in place.
- **Asking first:** after your first vote, Kino asks in its own words before iOS (or the browser) asks about notifications.

## Notes for the developer

- **The design file:** Figma has the whole system (variables in Dark and Light, text and effect styles, components), every flow built from those components, and a Motion section with each interaction animated in the prototype's timings, plus a timing table.
- **Sample data:** people, scores, takes, member numbers and where to watch are invented. Where to watch needs a provider (for example TMDB's watch providers, which come from JustWatch).
- **Backdrops:** a film page shows a real still when we can match one to its film for certain. Otherwise it shows the poster's colour with a field of dots, in the same place, for the film library to fill in.
- **What iOS decides:** push notifications use iOS's communication style, led by the sender's photo. iOS puts the app's icon on that photo's corner itself; the prototype draws the intent, a cream dot, the same "new" marker as the bell.
- **What the browser decides:** on the web, the browser shows its own notification prompt, and there are no contacts to ask for.
- **A take's menu:** it opens after a 0.52s hold, and moving more than 8px lets go (that's a scroll). Report needs a real moderation queue behind it.
- **Long lists:** only what's on screen animates (12 films at most), and posters past the first screenful load lazily. In the real build, virtualise long lists and page the feed in.
- **Motion:** two curves, Kino's ease (0.2, 0.7, 0.2, 1) and a small spring (0.3, 1.35, 0.5, 1); anything in your way stays under 0.6 seconds. Reduced motion turns it all off.

Film posters and stills belong to their studios and appear here for a non-commercial design study.
