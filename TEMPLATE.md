<img width="100%" alt="base" src=".cache/base.svg">
<%# await embed(`base`, { base: 'header, activity, community, repositories, metadata' }) _%>

<img width="100%" alt="languages" src=".cache/languages.svg">
<%# await embed(`languages`, { languages: true }) _%>

<img width="100%" alt="followup" src=".cache/followup.svg">
<%# await embed(`followup`, { followup: true }) _%>

<%- await include(`partials/rss.ejs`) %>

<img width="100%" alt="stars" src=".cache/stars.svg">
<%# await embed(`stars`, { plugin_stars: true }) _%>

<%- await include(`partials/topics.ejs`) %>

<img width="450" height="700" alt="Mastodon - Siavash's Toots" src=".cache/mastodon.svg">
<img width="450" height="700" alt="Twitter - Siavash's Tweets" src=".cache/twitter.svg">
