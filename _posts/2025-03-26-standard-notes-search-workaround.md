---
layout: post
title: Workaround for Missing in-note Search Feature of Standard Notes for Android
date: 2024-12-24
---

Standard Notes is a great note taking app. The killer feature for me is the end-to-end encryption feature. Only a couple of note taking apps have end-to-end encryption, and Standard Notes is one of them. It's also one of the first note taking apps to have this feature. It's **almost** perfect for me. 

I don't have that much demand from a note taking app. I don't like the idea of everything and a kitchen sink from a note taking app. It has to have this no-frill look and simple enough to quickly jot things down. All I want, from what I call a perfect note -aking app, is there in Standard Notes, except the individual note search functionality. 

They have the global search functionality on Standard Notes, but searching for in each note is still missing after so many years of its existence. It's one of the most requested features for Standard Notes. Yet the developers have yet to find a way to implement it. The lead developer Mo [said](https://github.com/standardnotes/forum/issues/330){:target="_blank"}:

>It's very, very hard. Searching is not the hard part. Showing a yellow rectangle behind instances of a text in a note is hard. It's hard because we use textarea for the Plain Editor which doesn't support any custom behavior, and it's hard because we'd also need to build a custom solution for every other editor in our ecosystem. The Bold Editor would need a different solution from the Plus Editor would need a different solution from the Spreadsheets editor, and so on. Then you need another custom solution for mobile native editors.
>
>In fact probably the only way to build this in the plain editor, which is the primary use case, would be to ditch textarea for a custom-render editor like CodeMirror, and this is no small feat.
>
>So no, none of this is easy.

Luckily, there's almost always a workaround. Just when I thougt of stop using Standard Notes for another, I found this solution for in-note searchability. This workaround is so simple that I felt stupid not to think about it before. 

The workaround is to open Standard Note from a mobile browser, like Chrome or Firefox, instead of using the app. So when you are using Standard Notes from a mobile browser, you can use the browser's built-it Find in page or search functionality, so it'll just work perfectly. You will get the search highlight for individual note in this way though that app itself doesn't have this feature. 

In-note search is so basic feature for a note-taking app for me that it made me look for alternative apps. But unfortunately the alternatives don't tick all the boxes. Especially the end-to-end encryption feature. This feature is important for me because sometimes I store passwords or other credentials in the note-taking app.

Without end-to-end encryption, the privacy and security of your note is left at the mercy of the people behind that note-taking or whichever app you're using. You need to trust them not to look at your credentials and passwords. You don't want the safety of your saved passwords dependent on this trust.