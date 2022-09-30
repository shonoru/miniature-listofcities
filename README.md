# Tutorial on how to get list of cities from wiki

Ref. https://ru.wikipedia.org/wiki/Список_городов_России

Choose element, right-click “Store as global variable” , and now you have temp1 in console


```
temp1
trs = temp1.getElementsByTagName('tr')

const cities = []

for (let tr of trs) {
    let td = tr.getElementsByTagName('td')[2]
    cities.push(td.textContent)
}

copy(JSON.stringify(cities))
```

Once copied, 

CTRL-V to any file, and save it with .json extension


NOTE: miniature prefix for smaller projects
