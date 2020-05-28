[![Netlify Status](https://api.netlify.com/api/v1/badges/300938da-634d-46d1-a676-2674c8279444/deploy-status)](https://app.netlify.com/sites/theracket/deploys)

# TheRacketPlaylistViewer

[The Racket Playlist Viewer](https://theracket.netlify.app/)

A simple site built using Vue.js and Vuetify that displays Triple J's [The Racket](https://www.abc.net.au/triplej/programs/the-racket/) showlist for a given date. I am using this app as a way to learn more about Vue.js and to provide an easy way for myself to listen to the shows contents after the show gets removed from the triple j website.

It utilises the following:
* Vue.js
* Vuetify
* axios
* moment.js 

## How
It makes http calls to the ABC Radio API to retrieve the show data - https://music.abcradio.net.au/api/v1/plays/search.json 
By using the following end point https://music.abcradio.net.au/api/v1/plays/search.json?station=triplej&from=${this.date}T12:00:00&to=${this.date}T15:00:00&limit=200&order=asc
we can get information (actuall a lot of information) on tracks played during the show.

I have included a link to youtube with search params prepopulated to listen to a song.

## The Racket Show
The Racket runs every Tuesday 10pm - 1am (Australian Eastern Standard Time) and plays an eclectic line-up of metal and its bulkiest subgenres, dipping into punk, post-rock and hardcore scenes, and even a little electro.

## To Do
* Take DST into account
* Provide a link to spotify web search
