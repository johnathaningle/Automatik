

> Note: we only record certain events. See `dom-events-to-record.js` in the code-generator folder for which events. This collection will be expanded in future releases.

## Usage
TBD
## Background

TBD

## Development

1. Run: `git clone https://github.com/checkly/Automatik.git`
2. Build the project: `cd Automatik && npm i && npm run dev`
2. Navigate to chrome://extensions
3. Make sure 'Developer mode' is checked
4. Click Load unpacked extension...
5. Browse to Automatik/build and click Select

## Cutting a Release

- bump versions in `package.json` and `manifest.json`
- tag the code with the version, i.e. `git tag v0.4.0`
- push with tags `git push --tags`

Now generate a release with **gren**. Make sure all issues associated with the new version are linked to a milestone
with the name of the tag.

```
gren release --override --data-source=milestones --milestone-match="{{tag_name}}"
```

## Credits & disclaimer

Automatic is a sister & love child to: 
[Automatik](https://github.com/checkly/Automatik), [Daydream](https://github.com/segmentio/daydream) and [ui recorder](https://github.com/yguan/ui-recorder).

## License
Apache 2
