# iSAQB Github Readme

This Github organisation holds repositories for the [iSAQB](https://isaqb.org), especially curricula, glossary and references.

In case of questions or suggestions, please contact:

* iSAQB technical support: support -at- isaqb -dot- org
* For Foundation-Level curricula and content: gs -at- gernotstarke -dot- de
* For the Advanced Level Curriculum Template: bwolf -at- isaqb -dot- org


## Release Process for Curricula

![Release process description for a curriculum, including the reasons for when to change which part of the release version](img/release_process.svg)


## How to Create a new Release of a Curriculum 

If a group of curators has decided that they want to create a new release, they have to do one of the following.

### Minor Release
Let's say there was a new release of a curriculum in 2024, then the git tag for the release will look like this: `2024.1-rev0`. 

To create a new minor release, all they have to do is to create a tag called `2024.1-rev1` and push it to the repository. GitHub workflows will automatically build and publish the new version. 

### Major Release
To create a new major release, they have to create a git tag called `2024.2-rev0`. It is important to reset the revision to 0 for consistent naming. Push it to the repository, and let GitHub workflows do their magic. 

### Completely New Release
If the curriculum is completely overhauled, the version number should be changed to the current year or the year when the release is supposed to be released, respectively. 

Before a release is created, the group of curators should create at least one release candidate. 
Let's say the last release is from 2023 (e.g. `2023.2-rev4`) and the group of curators would like to create a new release in 2025, then the tag name for the first release candidate would look like this: `2025.1-RC1` (Please note: Release candidates start at 1, compared to revisions which start at 0.)

Push it to the repository and a release candidate is created. The URL for the release candidate is 
`https://public.isaqb.orc/curriculum-NAME/release-candidate`. 

Once everyone is happy with the current release candidate, they need to create a new git tag called `2025.1-rev0` (in our example) and push it to GitHub, wait a few minutes, and then the new release is done. 

**Attention:** Once a new release is created, everything of the last release candidate is removed! 
