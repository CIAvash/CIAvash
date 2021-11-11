<%- await embed(`base`, { base: ['header', 'activity', 'community', 'repositories', 'metadata'] }) %>

<%- await embed(`lines`, { lines: true }) %>

<%- await embed(`languages`, { languages: true }) %>

<%- await embed(`followup`, { followup: true }) %>

<%- await include(`partial/rss.ejs`) %>

<%- await embed(`stars`, { stars: true }) %>
