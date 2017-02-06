[![License](https://img.shields.io/github/license/sharedlabs/sortable-list.svg?style=flat-square)](https://github.com/sharedlabs/file-uploader/blob/master/LICENSE.md)

# file-uploader

File uploader for multiple files with a progress bar.

It uses the [offthread-image](https://github.com/sharedlabs/offthread-image) element to render the thumbnails so it performs awesome on slow devices like mobile phones.

### Preview
![](https://media.giphy.com/media/l3q2wmnMfDGpVvnxK/giphy.gif)

### Use
```html
<file-uploader id="fileUploader"><file-uploader>

...
this.$.fileUploader.addFile(file, {url, method, headers});
```

### Browsers support

Any browser that supports Polymer 1.0
