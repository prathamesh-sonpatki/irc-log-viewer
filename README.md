## irc-log-viewer

This is a viewer for IRC logs which are stored in a CouchDB. It's basically a couchapp using Ember.js. Demo? Here you go: [http://emberjs.iriscouch.com/irc/_design/viewer/index.html](http://emberjs.iriscouch.com/irc/_design/viewer/index.html)

### Awesome stuff used

- [Ember.js](https://github.com/emberjs/ember.js)
- [BPM](https://github.com/bpm/bpm)
- [CouchDB](http://couchdb.apache.org/)

## Basic structure

The IRC messages saved in the CouchDB have the following format:

```javascript
{
   "user": {
       "id": "123",
       "name": "GOB"
   },
   "text": "Come on!",
   "date": "2012-12-21T12:34:56.789Z"
}
```

Inside the `_attachments` folder is the Ember.js app. The used views are located at [https://github.com/pangratz/irc-log](https://github.com/pangratz/irc-log)

## Development

### Prerequisites:
- installed BPM
- CouchDB where app can be deployed

### Develop

- Clone this repo
- Tests are in located in the `_attachments/tests` folder
- Execute `bpm preview` inside `_attachments`
- Access `localhost:4020/tests.html` to execute the tests