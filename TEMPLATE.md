<%- await embed(`base`, { base: "header, activity, community, repositories, metadata", config_output: png }) %>

<%- await embed(`lines`, { lines: true, config_output: png }) %>

<%- await embed(`languages`, { languages: true, config_output: png }) %>

<%- await embed(`followup`, { followup: true, config_output: png }) %>

**[📓 Repositories:](https://github.com/<%= user.login %>?tab=repositories)**
<%_ for (const { name, owner, isFork } of user.repositories.nodes) { _%>
  <%_ if (!isFork) _%>
    [<%= name %>](https://github.com/<%= `${owner.login}/${name}` %>) 
  <%_ } _%>
<%_ } _%>

<%- await include(`partials/rss.ejs`) %>

<%- await embed(`stars`, { stars: true, config_output: png }) %>
