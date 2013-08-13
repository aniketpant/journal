---
layout: post
title: Dependency managers no good.
date: 2013-05-29 09:08
---
I have been using composer and bower regularly. And they surely piss me off everytime I run them. They download the dependencies each time I run them and then they put them in a folder. The next time I run the same command in some other folder, it picks up some of the dependencies from the cache and the rest are downloaded all over again. **Why?** Why should this happen? Can't they work the way gems are installed? A folder named `.composer` and `.bower` located in `/home`. And each time I run a install, it will copy the content from these folders. And when I update, it will update the dependencies placed in these folders. Maybe I have been doing it wrong all along, or maybe these managers are actually wonky!
