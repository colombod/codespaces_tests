#  .NET Interactive code spaces test

Steps
 *  open this repo with code spaces
 *  install .NET Interactive Notebook extension
 *  open the browser develoepr tools
 *  open the COVID-19.dib file

Now the console output will show how the api is setup
![image](https://user-images.githubusercontent.com/375556/92963713-d37b3800-f46a-11ea-8c39-f45a4f0a1dab.png)

And the issue now si that the uri used in fetch will not return the javascript but an authentication challenge that at the end will redirect to the content.

```
https://github.com/login?return_to=https%3A%2F%2Fgithub.com%2Fcodespaces%2Fauth%2F1f2b55e9-d023-41ac-a41e-62a81dcc73da%3Fpath%3D%252fresources%252fdotnet-interactive.js%26query%3D%253fcacheBuster%253d1599849429679%26port%3D33209%26cid%3D9022302298382529f56085aba962154f
````

![image](https://user-images.githubusercontent.com/375556/92963765-e261ea80-f46a-11ea-89ee-c920f1afcc11.png)

This results in a cross-origin blocked calls
