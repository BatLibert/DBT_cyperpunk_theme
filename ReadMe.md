<h1 align="center">Welcome 👋</h1>

### 🏠 [Homepage](<%= projectHomepage %>)
<% } -%>
<% if (projectDemoUrl) { -%>

### ✨ [Demo](<%= projectDemoUrl %>)
<% } -%>
<% if (projectPrerequisites && projectPrerequisites.length) { -%>
![image](https://i.pinimg.com/originals/fa/dc/b2/fadcb24075acb650de29f258af69d830.gif)

## Prerequisites

<% projectPrerequisites.map(({ name, value }) => { -%>
- <%= name %> <%= value %>
<% }) -%>
<% } -%>
<% if (installCommand) { -%>

## Install

```sh
<%= installCommand %>
```
<% } -%>
<% if (usage) { -%>

## Usage

```sh
<%= usage %>
```
<% } -%>
<% if (testCommand) { -%>

## Run tests

```sh
<%= testCommand %>
```
<% } -%>
<% if (authorName || authorTwitterUsername || authorGithubUsername) { -%>

## Author
<% if (authorName) { %>
👤 **<%= authorName %>**
<% } %>
<% if (authorWebsite) { -%>
* Website: <%= authorWebsite %>
<% } -%>
<% if (authorTwitterUsername) { -%>
* Twitter: [@<%= authorTwitterUsername %>](https://twitter.com/<%= authorTwitterUsername %>)
<% } -%>
<% if (authorGithubUsername) { -%>
* GitHub: [@<%= authorGithubUsername %>](https://github.com/<%= authorGithubUsername %>)
<% } -%>
<% if (authorLinkedInUsername) { -%>
* LinkedIn: [@<%= authorLinkedInUsername %>](https://linkedin.com/in/<%= authorLinkedInUsername %>)
<% } -%>
<% } -%>
<% if (issuesUrl) { -%>

## 🤝 Contributing

Contributions, issues and feature requests are welcome!<br />Feel free to check [issues page](<%= issuesUrl %>). <%= contributingUrl ? `You can also take a look at the [contributing guide](${contributingUrl}).` : '' %>
<% } -%>

## Show your support

Give a ⭐️ if this project helped you!
<% if (authorPatreonUsername) { -%>

<a href="https://www.patreon.com/<%= authorPatreonUsername %>">
  <img src="https://c5.patreon.com/external/logo/become_a_patron_button@2x.png" width="160">
</a>
<% } -%>
<% if (licenseName && licenseUrl) { -%>

## 📝 License

<% if (authorName && authorGithubUsername) { -%>
Copyright © <%= currentYear %> [<%= authorName %>](https://github.com/<%= authorGithubUsername %>).<br />
<% } -%>
This project is [<%= licenseName %>](<%= licenseUrl %>) licensed.
<% } -%>

***
