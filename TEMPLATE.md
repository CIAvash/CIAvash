<%- await embed(`base`, { base: 'header, activity, community, repositories, metadata' }) %>

<%- await embed(`lines`, { plugin_lines: true }) %>

<%- await embed(`languages`, { plugin_languages: true }) %>

<%- await embed(`followup`, { plugin_followup: true }) %>

<%- await include(`partials/rss.ejs`) %>

<%- await embed(`stars`, { plugin_stars: true }) %>
