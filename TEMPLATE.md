<%- await embed(`base`, { base: "header, activity, community, repositories, metadata" }) %>

<%- await embed(`lines`, { lines: true }) %>

<%- await embed(`languages`, { languages: true }) %>

<%- await embed(`followup`, { followup: true }) %>

<%_ if (plugins.repositories) { _%>
**[📓 Repositories](https://github.com/<%= user.login %>?tab=repositories)**
  <%_ if (plugins.repositories.error) { _%>
    <%= plugins.repositories.error.message _%>
  <%_ } else if (plugins.repositories.length) { _%>
     <%_ for (const { owner, name } of plugins.repositories) { _%>
       [<%= name %>](https://github.com/<%= `${owner}/${name}` %>) 
     <%_ } _%>
  <%_ } else { _%>
     No repositores
  <%_ } _%>
<%_ } _%>

<%- await include(`partials/rss.ejs`) %>

<%- await embed(`stars`, { stars: true }) %>
