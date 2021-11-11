<%- await embed(`base`, { base: 'header, activity, community, repositories, metadata' }) %>

![languages](.cache/languages.svg)
<%# await embed(`languages`, { languages: true }) %>

<%- await embed(`followup`, { followup: true }) %>

<%- await include(`partials/rss.ejs`) %>

![stars](.cache/stars.svg)
<%# await embed(`stars`, { plugin_stars: true }) %>
