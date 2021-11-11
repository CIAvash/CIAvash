![base](.cache/base.svg)
<%# await embed(`base`, { base: 'header, activity, community, repositories, metadata' }) #%>

![languages](.cache/languages.svg)
<%# await embed(`languages`, { languages: true }) _%>

![followup](.cache/followup.svg)
<%# await embed(`followup`, { followup: true }) _%>

<%- await include(`partials/rss.ejs`) %>

![stars](.cache/stars.svg)
<%# await embed(`stars`, { plugin_stars: true }) _%>
