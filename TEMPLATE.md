<%- await embed(`base`, { base: 'header, activity, community, repositories, metadata' }) %>

<%- await embed(`lines`, { lines: true, config_output: 'png' }) %>

<%- await embed(`languages`, { languages: true, config_output: 'png' }) %>

<%- await embed(`followup`, { followup: true }) %>

<%- await include(`partials/rss.ejs`) %>

<%- await embed(`stars`, { stars: true, config_output: 'png' }) %>
