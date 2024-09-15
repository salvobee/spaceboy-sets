# Vinyl Mixtape Player

A simple webpage that simulates a vinyl record spinning while playing mixtapes. The mixtapes are stored on S3 and served via CloudFront.

## Features

- Vinyl record spins when the audio plays.
- Dropdown menu to select mixtapes.
- Responsive design, adapting to different screen sizes.

## How to Use

1. **Upload Mixtapes**:

   - Upload your mixtape files to S3.
   - Update the `mixtapes.json` file with the URLs and titles of the mixtapes.

2. **Run Locally**:
   Simply open `index.html` in your browser. No build tools required.

3. **Deploy**:
   - If you're using Firebase Hosting, put everything in a `public/` folder.
   - Run `firebase deploy` to go live.

## JSON Format for Mixtapes

The `mixtapes.json` file should look like this:

```json
[
  {
    "title": "Mixtape 1",
    "url": "https://d3lrnnt7lnzh9p.cloudfront.net/mixtape1.mp3"
  },
  {
    "title": "Mixtape 2",
    "url": "https://d3lrnnt7lnzh9p.cloudfront.net/mixtape2.mp3"
  }
]
```
