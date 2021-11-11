<%- await embed(`base`, { base: "header, activity, community, repositories, metadata" }) %>

<%- await embed(`lines`, { lines: true, config_output: "markdown", config_base64: false, markdown_cache: ".cache" }) %>

<%- await embed(`languages`, { languages: true, config_output: "markdown", config_base64: false, markdown_cache: ".cache" }) %>

<%- await embed(`followup`, { followup: true, config_output: "markdown", config_base64: false, markdown_cache: ".cache" }) %>

**[📓 Repositories:](https://github.com/<%= user.login %>?tab=repositories)**
<%_ for (const { name, owner } of user.repositories.nodes) { _%>
    [<%= name %>](https://github.com/<%= `${owner.login}/${name}` %>)
<%_ } _%>

<%- await include(`partials/rss.ejs`) %>

<%- await embed(`stars`, { stars: true, config_output: "markdown", config_base64: false, markdown_cache: ".cache" }) %>
