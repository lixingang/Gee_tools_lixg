## 启动全部任务：
```
function runTaskList(){
    var tasklist = document.getElementsByClassName('task local type-EXPORT_IMAGE awaiting-user-config');
    for (var i = 0; i < tasklist.length; i++)
            tasklist[i].getElementsByClassName('run-button')[0].click();
}


function confirmAll() {
    var ok = document.getElementsByClassName('goog-buttonset-default goog-buttonset-action');
    for (var i = 0; i < ok.length; i++)
        ok[i].click();
}

runTaskList();
confirmAll();
```

## 停止全部任务
```
function stopTaskList(){
    var tasklist = document.getElementsByClassName('task remote type-EXPORT_IMAGE submitted-to-backend');
    for (var i = 0; i < tasklist.length; i++)
            tasklist[i].getElementsByClassName('indicator')[0].click();
}

function confirmAll() {
    var ok = document.getElementsByClassName('goog-buttonset-default goog-buttonset-action');
    for (var i = 0; i < ok.length; i++)
        ok[i].click();
}
stopTaskList();
confirmAll();
```
