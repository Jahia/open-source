<a href="https://www.jahia.com/">
    <img src="https://www.jahia.com/modules/jahiacom-templates/images/jahia-3x.png" alt="Jahia logo" title="Jahia" align="right" height="60" />
</a>

# Open-Source @ Jahia

Jahia has a long history of contribution to Open-Source, you will find in this repository resources to help you discover our product, its codebase, and our open-source practices. 

## Discover

Jahia GitHub organization has a fairly large number of open-source repositories, and many new ones get created every week. With the exception of some of the legacy parts of the codebase, each of our Jahia modules have their own repository, named identically (or similarly) to the module ID. 

You can also repository topics available from [Jahia Organization](https://github.com/Jahia) (right side of the screen) to quickly access the [list of product modules](https://github.com/search?q=topic%3Aproduct+org%3AJahia). 

## Licenses

Historically Jahia has been distributing its codebase under a dual licensing model using GPLv3, and Jahia's JSEL (Enterprise) license. As the software (and the open-source) industry evolves, we are taking steps towards modernizing our practices. 

Over the past few months, we've been taking the time to review our practices and refine our Open-Source strategy moving forwards. As a result, our codebase will progressively be moving away from dual-licensing towards more permissive licenses to encourage others to contribute and build on top of our products.

In the future, our license of choice for our Open-Source codebase will be [Apache version 2.0](https://www.apache.org/licenses/LICENSE-2.0), with some of our front-end oriented components distributed under [MIT](https://opensource.org/licenses/MIT). 

Watch for the `LICENSE` file in each of our repository to better understand which license currently applies to the codebase.

## Contribute

Alongside work taking place on our Open-Source strategy, we are currently actively working at revising (and clarifying) our contributing guidelines. Expect more in the coming months.

## Fork

Although we encourage developers to first submit issues (and subsequently Pull-Requests) to our supported codebases (core or modules), there might come a time when a divergence of vision for the future of a module would result in [forking](https://en.wikipedia.org/wiki/Fork_(software_development)). 

May the decision to fork be taken, Jahia recommends the following practices:
* Update the module group ID, for example by changing it from `org.jahia.modules` to `org.jahiacommunity.modules`
* Bump up your first release to the next major version, for example if the last module release was `2.4.0`, the first forked release could be `3.0.0`.
* Prefer [GitHub Fork](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo) feature, instead of creating a new repository and copying the code. This would allow users and developers to find your fork by navigating through Jahia's organization.
* Don't forget to include changelog notes, to make it easy for future consumers of your forked module to understand how it diverges from Jahia's.

## Community

Over the years, Jahia has built a community of passionate users and developers. You can find more details about how Jahia is supporting the community on the [Academy](https://academy.jahia.com/community)

### Modules development

Jahia welcomes the community to take over active development of modules Jahia no-longer officially supports. Such modules and their corresponding codebases can easily be found using the [community topic](https://github.com/search?q=topic%3Acommunity+org%3AJahia).

Do not hesitate to reach-out if you would like your forked module to be listed in the readme of the community module.

## Jahia internal

The following section is aimed at being used by Jahia employees and is detailed here to provide insights about our internal processes.

## Modifying a license or repository visibility

Modifying a license or changing the repository visibility (PUBLIC / PRIVATE) is a sensitive topic and it is critical to make sure that such a decision is supported at a company level.

Please create a ticket in the [OPENCODE project](https://jira.jahia.org/projects/OPENCODE/issues), a template will assist you in populating the ticket with the necessary details. You can reach out to the [Open-Source team on slack](https://jahia.slack.com/archives/CRNNE2J6T) may you have questions.

If you're converting an Enterprise module to Open-Source and, once approval has been obtained in the OPENCODE ticket, please make sure the new repository's contains, at a minimum:

* A Readme with the Open-Source footer as available in [this sample](./README_OpenSource.md)
* A `LICENSE` file (Apache2 or MIT)

## End of Support

As mentioned earlier in this document, there might come a time when Jahia's product team decides to stop supporting an Open-Source or Enterprise module and halt its active development. 

The process below details the steps to be following in such situations:

### Open-Source module

* Make sure the license is properly set (Apache2 or MIT)
* Make sure the repository readme contains the "Open-Source" section and create the "Archived" section [see this sample](./README_Archived.md)
* Update the repository's topics, remove "supported" and add "community"
* Archive the repository

### Enterprise module

* Create an [OPENCODE](https://jira.jahia.org/projects/OPENCODE/issues) ticket to enquire whether this module can be made Open-Source
* If NO: Archive the repository
* If YES:
  * Convert the module's license to either Apache2 or MIT
  * Update the Repository's readme with the "Open-Source" and "Archived" sections
  * Update the repository's topics, remove "supported" and add "community"
  * Archive the repository
