<%- await embed(`img-base`, { 'base': 'header, activity, community, repositories, metadata' }) -%>

<%- await embed(`img-lines`, { 'lines': true }) -%>

<%- await embed(`img-languages`, { 'languages': true }) -%>

<%- await embed(`img-followup`, { 'followup': true }) -%>

<%- await include(`partials/rss.ejs`) -%>

<%- await embed(`img-stars`, { 'stars': true }) -%>
