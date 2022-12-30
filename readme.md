# WMGFT FediBot

## Todo
[ ] Parse Phab tasks and generate JSON
[ ] Manually add hashtags to JSON
[ ] Randomly select task from JSON and generate post
[ ] Toot!

## Generate JSON
Read https://phabricator.wikimedia.org/maniphest/query/u8k6X70S9euJ/#R and extract some elements into a JSON file:

```json
{
	"T319097": {
		"title": "mwbot-rs: Split up node.rs",
		"url": "https://phabricator.wikimedia.org/T319097",
		"hashtags": [
			"rust"
		]
	}
}
```
Phab task ID (CSS class selector `.phui-oi-objname`) and title (CSS class selector `.phui-oi-link`) should be pretty easy to grab, hashtags (really just the programming language) will need to be manually added afterwards.

