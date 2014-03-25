# jira-cli+OSX Keychain


This is a command line client for jira, because no one likes their terrible
interface.

This fork uses node-keytar to store credentials in the OSX keychain as opposed to plain text.



## Getting Started

*  Install the module with: `npm install -g https://github.com/startswithaj/jira-cli`
*  Run it with `jira`

## What does it do?

*  Lists all a user's issues
*  List all a user's projects
*  Finds an issue by Key (AB-123) or Id (123456)
*  Opens an issue 
*  Allows user to add a new ticket to different projects
*  Transitions an issue (shows all available transition states)
*  Adds a worklog to an issue
*  Allow searching to be limited by project id

## TODO

*  PROFIT?
*  MOAR testing

## Documentation ##

[GitHub Documentation](http://tebriel.github.com/jira-cli/)

## Examples ##

`jira -l`

`jira -f AB-123`

## Notes ##

If you use `https:` for jira, add `"protocol": "https:"` to your .jiraclirc.json
If your ssl certs are also self-signed add: `"strictSSL": false` to your .jiraclirc.json

## Testing ##

Using jasmine-node with grunt currently. Tests are a bit silly, but they helped
me learn jasmine spies. So that's good.

## Contributing

In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [grunt](https://github.com/gruntjs/grunt).


## Release History

*  _0.5.0 Changing list (`-l`) to to use the query `resolution = unresolved` (Thanks
   to [zowens](https://github.com/zowens))_
*  _0.4.1 Accidentally quitting before callback was finished_
*  _0.4.0 Now able to ignore self-signed SSL Certs and specify protocol_
*  _0.3.1 Fixed some bugs_
*  _0.3.0 Updated version of jira_
*  _0.2.9 Fixed an issue where special characters were in the username_
*  _0.2.8 Fixed issue with create that would prevent you from creating_
*  _0.2.7 Fixed typo that prevented -w from working_
*  _0.2.6 Now takes -o to limit to specific project(s)_
*  _0.2.5 Now normalizing event types and item types_
*  _0.2.4 I did something here, don't remember_
*  _0.2.3 Fixed an issue where invalid input caused an exception_
*  _0.2.2 Added wordrap to -d so that the text is easier to grok_
*  _0.2.1 Added -d flag to show details for list/find_
*  _0.2.0 Refactored organization. Creates config file if not present_
*  _0.1.9 Defaults for project in config, lists others if desired_
*  _0.1.8 Now allows entry of worklog when transitioning items, or by itself_
*  _0.1.7 Now requiring my custom npm module for node-jira-devel_
*  _0.1.6 Transitioning now shows all available options_
*  _0.1.5 Listing Id for project_
*  _0.1.4 Listing Types in Create_
*  _0.1.3 Listing Projects_
*  _0.1.2 Moar Minor Doc Changes_
*  _0.1.1 Minor Doc Changes_
*  _0.1.0 Initial Release_

## License

Copyright (c) 2012 Chris Moultrie  
Licensed under the MIT license.
