<%- await embed(`base`, { base: "header, activity, community, repositories, metadata", config_output: png }) %>

<%- await embed(`lines`, { lines: true, config_output: png }) %>

<%- await embed(`languages`, { languages: true, config_output: png }) %>

<%- await embed(`followup`, { followup: true, config_output: png }) %>

<%_ } if (plugins.repositories.length) { _%>
**[📓 Repositories](<%= user.html_url %>?tab=repositories)**
     <%_ for (const { owner, name } of computed.repositories) { _%>
       [<%= name %>](https://github.com/<%= `${owner}/${name}` %>) 
     <%_ } _%>
<%_ } _%>

<%- await include(`partials/rss.ejs`) %>

<%- await embed(`stars`, { stars: true, config_output: png }) %>
