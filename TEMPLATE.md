<%- await embed(`base`, { base: 'header, activity, community, repositories, metadata' }) %>

![lines](.cache/lines.svg)

<%# await embed(`lines`, { plugin_lines: true }) %>

![languages](.cache/languages.svg)

<%# await embed(`languages`, { plugin_languages: true }) %>

<%- await embed(`followup`, { plugin_followup: true }) %>

<%- await include(`partials/rss.ejs`) %>

![stars](.cache/stars.svg)

<%# await embed(`stars`, { plugin_stars: true }) %>
