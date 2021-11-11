<%- await embed(`base`, { base: "header, activity, community, repositories, metadata", config_output: png }) %>

<%- await embed(`lines`, { lines: true, config_output: png }) %>

<%- await embed(`languages`, { languages: true, config_output: png }) %>

<%- await embed(`followup`, { followup: true, config_output: png }) %>

<%- await include(`partials/rss.ejs`) %>

<%- await embed(`stars`, { stars: true, config_output: png }) %>
