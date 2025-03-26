---
layout: post
title: Workaround for Missing in-note Search Feature of Standard Notes for Android
date: 2024-12-24
---

[Standard Notes](https://standardnotes.com/){:target="_blank"} is a great note taking app. The killer feature for me is it's end-to-end encryption feature. Only a couple of note taking apps have end-to-end encryption till date. 

I don't have that much demand from a note taking app. I don't like the idea of a note-taking app being everything and a kitchen sink. It has to have this no-frills look and be simple enough to quickly jot things down. All I want from what I call a perfect note-taking app is there in Standard Notes, except the in-note search functionality. 

They have the global search functionality on Standard Notes, but searching inside individual note is still missing after so many years of its existence. It's one of the most requested features for Standard Notes. Yet the developers have yet to find a way to implement it. [According to the lead developer Mo](https://github.com/standardnotes/forum/issues/330#issuecomment-863272902){:target="_blank"}:

>It's very, very hard. Searching is not the hard part. Showing a yellow rectangle behind instances of a text in a note is hard. It's hard because we use textarea for the Plain Editor which doesn't support any custom behavior, and it's hard because we'd also need to build a custom solution for every other editor in our ecosystem. The Bold Editor would need a different solution from the Plus Editor would need a different solution from the Spreadsheets editor, and so on. Then you need another custom solution for mobile native editors.
>
>In fact probably the only way to build this in the plain editor, which is the primary use case, would be to ditch textarea for a custom-render editor like CodeMirror, and this is no small feat.
>
>So no, none of this is easy.

Luckily, there's almost always a workaround. Just when I thought of stop using Standard Notes for the alternatives, I found this solution for in-note searchability on Android. I should mention that, the in-note feature is there to some extent for the paid users, but not for the free users. So you gotta find a way. 

The workaround is so simple that I felt stupid not to think of it earlier. It's to open Standard Note from a mobile browser, like Chrome or Firefox, instead of using the app. So when you are using Standard Notes from a mobile browser, you can use that browser's built-it Find in page or search functionality. It's almost a perfect solution. You will get the search highlight for individual note in this way though the app itself doesn't have this feature. Yet.

In-note search is so basic a feature for a note-taking app that, absence of it in Standard Notes made me look for the alternatives. But unfortunately the alternatives didn't tick all the boxes. Especially when it came to the end-to-end encryption feature. 

End-to-end encryption is important for me because sometimes I store passwords and other credentials in the note-taking app. Without the end-to-end encryption, the privacy and security of your notes are left at the mercy of the people behind that note-taking or whichever app you're using. You need to trust them not to look at your credentials and passwords. You don't want the safety of your saved passwords dependent on this trust alone.