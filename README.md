# jira-cli

A command line client for jira.

## Install
```bash
npm install -g https://github.com/johnathankent/jira-cli
```

## Features
*  Lists all a user's issues
*  List all a user's projects
*  Finds an issue by Key (AB-123) or Id (123456)
*  Opens an issue
*  Allows user to add a new ticket to different projects
*  Transitions an issue (shows all available transition states)
*  Adds a worklog to an issue
*  Allow searching to be limited by project id

## Config

### Self Signed SSL certs
If your ssl certs are also self-signed add: `"strictSSL": false` to `~/.jiraclirc`

## Testing
* Using jasmine-node with grunt.
* Lint and test your code using [grunt](https://github.com/gruntjs/grunt).

## Contributing
* Maintain the existing coding style.
* Add unit tests for any new or changed functionality.

## License

[MIT license](LICENSE.md)
