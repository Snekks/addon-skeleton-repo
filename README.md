
# Repository Explanation

## Benefits
### Addon Discovery
By using the polymorph config file, Polymorph can turn your repository into being the owner of what you display. No more configuring data across multiple applications! Add / Modify polymorph.yaml and you're 100% done.

## polymorph.yaml - Explained
### Identifier
This is a unique identifier specific to your addon. It drives the addon discovery and ties your addon to its repository. This should never be modified. The value provided to you is all you need.

### LogoPath
Increase your discoverability with a cool logo! This is just a string of the path from your provided **Discovery Reference**. For example, I have a logo I want to provide (as well as screenshots) - I'll add a folder called media to my repository in my **Discovery Reference**'d branch. Within it, I'll add a png file called logo.png.
#### Example

    LogoPath: /media/logo.png

### Category
This increases discoverability when a user searches based on category. One of the following strings:   Raiding, PvP, Map, Inventory, RolePlay, PvE, Unit Frames, TradeSkill, Auction House, Action Bars, Chat, Class & Role, Suites, Misc
#### Example

    Category: PvE

### Summary
A brief blurb about your addon. Limited to 256 characters.
#### Example

    Summary: This addon is the greatest addon ever made. It does stuff.

### OverviewPath
The path to a markdown file you would like users to see when viewing your addon. Common uses would be a readme.md. 
#### Example

    OverviewPath: readme.md

### SecondaryAuthors
If you have other people who have contributed to your addon and you want to give them credit, list them here.
#### Example

    SecondaryAuthors: Varian Wrynn, Garrosh Hellscream, Dan

### DocumentationUrl:
An URL pointed to your documentation / help if you have it.
#### Example

    DocumentationUrl: https://github.com/Snekks/addon-skeleton-repo/wiki

### IssueTrackingUrl:
An URL pointed to your issue tracking if you have it.
#### Example

    IssueTrackingUrl: https://github.com/Snekks/addon-skeleton-repo/issues

### Media
Screenshots are important for promoting your addon! Up to 15 screenshots can be provided. Unlike the LogoPath, Media allows you to add a name and description to your images. But like the LogoPath, each image requires a ImagePath property which is the path to the image within your **Discovery Reference**'d branch. 
#### Example
    Media:
	    - ImagePath: /media/image1.png
	      Name: Cool screenshot
	      Description: This is a cool screenshot of my addon
	    - ImagePath: /media/image2.jpg
	      Name: Cooler screenshot
	      Description: Yeah, this is great!

### LatestVersion
By providing the latest version (latest version tag), users will be able to gather the correct tag attached to your latest release. Sometimes tags aren't always as they seen with what is considered 'ready for consumers'. By providing the latest version tag, it's guaranteed a user always gets the latest version you expect them to.
#### Example

    LatestVersion: 1.0.4

### LatestPreReleaseVersion
By providing this property, users can download pre-releases (alpha / beta if you will). As an example, if you as an author are working on a PTR or new expansion build, you can provide that tag.
#### Example

    LatestPreReleaseVersion: 2.0.1-ptr.1

