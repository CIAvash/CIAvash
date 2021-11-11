<%- await embed(`base`, { base: 'header, activity, community, repositories, metadata' }) %>

<%- await embed(`languages`, { languages: true }) %>

<%- await embed(`followup`, { followup: true }) %>

<%- await include(`partials/rss.ejs`) %>

<%- await embed(`stars`, { plugin_stars: true }) %>
