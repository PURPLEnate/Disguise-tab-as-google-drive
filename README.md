# Disguise-tab-as-google-drive
Disguises the icon and name of the tab you're on with the icon and name given in the code

Setup: Create a bookmark, copy the provided code and paste it in as the URL (name it whatever you want):


javascript:(function() {
var link = document.querySelector("link[rel*='icon']") || document.createElement('link');
link.type = 'image/x-icon';link.rel = 'shortcut icon';
link.href = 'https://ssl.gstatic.com/docs/doclist/images/infinite_arrow_favicon_5.ico';
document.title = 'My Drive - Google Drive';
console.log(document.title);
document.getElementsByTagName('head')[0].appendChild(link);})();

