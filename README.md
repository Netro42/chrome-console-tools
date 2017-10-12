# Chrome Console Tools
A list of useful chrome console scripts

## Download a list of all network requests by domain

An extremely handy recipe for when you want to make a DNS prefetch file

- Go to your network tab in chrome inspector
- Now inspect _that_ (either right clicking, keyboard shortcuts or using file menu system)
- Type the following command

`UI.panels.network._networkLogView._dataGrid._rootNode.dataGrid._rootNode.dataGrid._rootNode._flatNodes.map(n => n._request._parsedURL.host).join('\n');`

or

`copy(UI.panels.network._networkLogView._dataGrid._rootNode.dataGrid._rootNode.dataGrid._rootNode._flatNodes.map(n => n._request._parsedURL.host).join('\n'));`

if you want it in your clipboard.



## Download a list of all network requests by url

- Go to your network tab in chrome inspector
- Now inspect _that_ (either right clicking, keyboard shortcuts or using file menu system)
- Type the following command

`UI.panels.network._networkLogView._dataGrid._rootNode.dataGrid._rootNode.dataGrid._rootNode._flatNodes.map(n => n._request._url).join('\n');`

or

`copy(UI.panels.network._networkLogView._dataGrid._rootNode.dataGrid._rootNode.dataGrid._rootNode._flatNodes.map(n => n._request._url).join('\n'));`

if you want it in your clipboard

