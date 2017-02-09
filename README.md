[![License](https://img.shields.io/github/license/sharedlabs/sortable-list.svg?style=flat-square)](https://github.com/sharedlabs/file-uploader/blob/master/LICENSE.md)

# file-uploader

File uploader for multiple files with a progress bar.

It uses the [offthread-image](https://github.com/sharedlabs/offthread-image) element to render the thumbnails so it performs awesome on slow devices like mobile phones.

### Preview (Uploading files to Amazon S3)
![](http://i.giphy.com/l0ExvurNrcBCmwaFa.gif)

### Use
```html
<file-uploader id="fileUploader"><file-uploader>

...
const xhrParamsPromise = new Promise((resolve, reject) => {
  ...
  resolve({url, method, headers});
});

this.$.fileUploader.addFile(file, xhrParamsPromise);
```

Why xhrParams as a promise? This is handy on enviroments like S3 when you have to ask for signed urls before uploading the files. This way that request is also part of the file uploading progress.

### Browsers support

Any browser that supports Polymer 2.0-preview
