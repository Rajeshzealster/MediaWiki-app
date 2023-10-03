# MediaWiki-app
Modelling and Dynamic deployment of MediaWiki app, an open-source server-based wiki application distributed under the GNU General Public License (GPL).

MediaWiki is an open-source server-based wiki application distributed under the GNU General Public License (GPL). It is widely recognized as the software that powers Wikipedia. MediaWiki is a robust and expandable platform that uses PHP for data processing and presentation and relies on databases like MySQL for information storage. This platform is designed for websites that experience high daily traffic volumes.

## Key Features

- **Collaborative Authoring:** MediaWiki enables concurrent editing by multiple users, making it ideal for constructing knowledge repositories and comprehensive documentation that require contributions from diverse individuals.

- **Revision History:** Every modification made to a MediaWiki page is meticulously logged, allowing you to review the complete edit history. This feature is invaluable for tracking changes, identifying contributors, and reverting to previous versions when needed.

- **Structured Content:** MediaWiki empowers the establishment of methodically organized content through the utilization of templates and categorization, ensuring systematic and uniform information arrangement.

- **User Administration:** MediaWiki incorporates user management functionalities, allowing administrators to regulate editing, authoring, and viewing privileges based on user roles and authorizations.

- **Search Efficiency:** MediaWiki boasts a potent search engine, enabling users to swiftly retrieve information within a wiki, which is crucial for extensive knowledge databases and documentation systems.

- **Expansions and Tailoring:** MediaWiki offers extensive support for augmentations and add-ons, allowing for the integration of supplementary features, such as discussion forums and multimedia support, making it adaptable to meet precise requirements.

## How MediaWiki Operates

MediaWiki functions through a structured process, enabling users to craft and revise wiki pages employing a simplified markup language. Here's a fundamental overview:

1. **Editing:** Users initiate the editing process by clicking on the "Edit" button, granting them access to modify page content using a simplified markup language similar to HTML.

2. **Version Management:** Each edit results in the creation of a new page version, preserving the historical evolution of the content. Users can compare different versions and identify contributors.

3. **Discourse:** MediaWiki commonly integrates discussion pages where users can engage in dialogues concerning modifications and offer feedback pertinent to the content.

4. **Categorization and Templates:** Users categorize pages based on content themes and leverage templates to ensure uniform layout and formatting throughout the entire wiki.

5. **User Profiles and Permissions:** User accounts may be established to monitor contributors' activities, and administrators configure permissions.

6. **Search Functionality:** MediaWiki incorporates a built-in search engine, empowering users to swiftly locate desired content within the wiki.

7. **Extensions:** Additional functionality can be incorporated into the wiki through the utilization of extensions and plugins.

## Deployment with TOSCA

MediaWiki can be deployed using TOSCA (Topology and Orchestration Specification for Cloud Applications). The prototype as shown in below figure consists of two physical nodes: one as an HTTP server hosting the MediaWiki application, and the other hosting a database serving as the central repository for content, user data, version history, and metadata.
![Uploading Service_design_blueprint (2).png…]()


- **TOSCA Modeling:** The MediaWiki application is modeled in a TOSCA service template, and dynamic deployment is facilitated by xOpera, a TOSCA-compliant orchestrator. xOpera uses Ansible playbooks for implementation and SSH for remote machine connections.

- **Orchestration Process:** xOpera analyzes relationships and dependencies between components in the TOSCA templates, using a graph-based execution engine to ensure proper deployment and configuration.
  ![mediawiki_orchestration](https://github.com/Rajeshzealster/MediaWiki-app/assets/97143348/a5ba6791-c015-4264-8d77-e4cbe1475902)


MediaWiki, with its collaborative authoring, structured content organization, and extensive customization options, continues to be an indispensable tool for knowledge collection and organization, serving numerous websites, corporations, and organizations.

For detailled deployment commands offered by xOpera, visit [xOpera CLI](https://xlab-si.github.io/xopera-docs/02-cli.html)

## Contributing

If you would like to contribute to this project, please open an issue or submit a pull request. We welcome your contributions.


## Contact

For questions or feedback, feel free to contact the project maintainer:
- Rajesh Thalla - <rajeshzealster@gmail.com>
