<%- await embed(`base`, { base: "header, activity, community, repositories, metadata" }) %>

<%- await embed(`lines`, { lines: true }) %>

<%- await embed(`languages`, { languages: true }) %>

<%- await embed(`followup`, { followup: true }) %>

<%- await include(`partials/repositories.ejs`) %>

<%- await include(`partials/rss.ejs`) %>

<%- await embed(`stars`, { stars: true }) %>
