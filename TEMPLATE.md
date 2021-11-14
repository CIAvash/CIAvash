<img style="width: 100%" alt="base" src=".cache/base.svg">
<%# await embed(`base`, { base: 'header, activity, community, repositories, metadata' }) _%>

<img style="width: 100%" alt="languages" src=".cache/languages.svg">
<%# await embed(`languages`, { languages: true }) _%>

<img style="width: 100%" alt="followup" src=".cache/followup.svg">
<%# await embed(`followup`, { followup: true }) _%>

<%- await include(`partials/rss.ejs`) %>

<img style="width: 100%" alt="stars" src=".cache/stars.svg">
<%# await embed(`stars`, { plugin_stars: true }) _%>
