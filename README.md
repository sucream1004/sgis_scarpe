# primitive scraping
## for loop
[JS for loop](https://www.w3schools.com/js/js_loop_for.asp) \
[JQuery $.each](https://api.jquery.com/each/)
```
#Finder
$('#location_mapNavi_1').click();

#Class selector

#Seoul
$('.li-strong').eq(0).click();
#Gu = 18 ~ 42
$('.li-strong').eq(18).click();
#Dong = 44 ~ $('.li-strong').length - 1 p.s. 43 is all Dong.
$('.li-strong').eq(44).click();

#double click the condition
$('#API_4011-0 > div.text').dblclick();

#year 2000
$('#div_y2000').click();
#year 2005
$('#div_y2005').click();
#year 2010
$('#div_y2010').click();
#year 2015
$('#div_y2015').click();
#year 2016
$('#div_y2016').click();
#year 2017
$('#div_y2017').click();

#download
$('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();

#hmm..
$('#navi-confirm').click()

$('#div_y2017').click();
$('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();

#Set the time
setTimeout(function(){
    // code here
}, 3000);
```
```
############################## EXAMPLE 개포동 2000~2015 ######################################

$('.li-strong').eq(0).click();

setTimeout(function(){
    $('.li-strong').eq(18).click();
}, 3000);

setTimeout(function(){
    $('.li-strong').eq(44).click();
}, 6000);

setTimeout(function(){
    $('#navi-confirm').click()
}, 9000);

setTimeout(function(){
    $('#btnList_1').click();
}, 12000);

setTimeout(function(){
    $('#API_0302-1').dblclick();
}, 15000);

setTimeout(function(){
    $('#div_y2000').click();
}, 18000);

setTimeout(function(){
    $('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();
}, 21000);

setTimeout(function(){
    $('#div_y2005').click();
}, 24000);

setTimeout(function(){
    $('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();
}, 27000);

setTimeout(function(){
    $('#div_y2010').click();
}, 30000);

setTimeout(function(){
    $('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();
}, 33000);

setTimeout(function(){
    $('#div_y2015').click();
}, 36000);

setTimeout(function(){
    $('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();
}, 39000);

setTimeout(function(){
    $('#div_y2016').click();
}, 42000);

setTimeout(function(){
    $('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();
}, 45000);

setTimeout(function(){
    $('#div_y2017').click();
}, 48000);

setTimeout(function(){
    $('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();
}, 51000);
```

## Range Function
[Range Function Source](https://stackoverflow.com/questions/8273047/javascript-function-similar-to-python-range)
```
function range(start, stop, step) {
    if (typeof stop == 'undefined') {
        // one param defined
        stop = start;
        start = 0;
    }

    if (typeof step == 'undefined') {
        step = 1;
    }

    if ((step > 0 && start >= stop) || (step < 0 && start <= stop)) {
        return [];
    }

    var result = [];
    for (var i = start; step > 0 ? i < stop : i > stop; i += step) {
        result.push(i);
    }

    return result;
};
```
## 동동
```
var dong = range(44, $('.li-strong').length)
$.each(dong, function (j, m) {
    $('.li-strong').eq(0).click();
    setTimeout(function () {
        $('.li-strong').eq(18).click();
    }, 3000 + j*51000);
    setTimeout(function () {
        $('.li-strong').eq(m).click();
    }, 6000 + j*51000);
    setTimeout(function () {
        $('#navi-confirm').click();
    }, 9000+ j*51000  );
    setTimeout(function () {
        $('#btnList_1').click();
    }, 12000+ j*51000  );
    setTimeout(function () {
        $('#API_4011-0').dblclick();
    }, 15000 + j*51000 );
    setTimeout(function () {
        $('#div_y2000').click();
    }, 18000 + j*51000 );
    setTimeout(function () {
        $('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();
    }, 21000 + j*51000 );
    setTimeout(function () {
        $('#div_y2005').click();
    }, 24000 + j*51000 );
    setTimeout(function () {
        $('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();
    }, 27000 + j*51000 );
    setTimeout(function () {
        $('#div_y2010').click();
    }, 30000 + j*51000 );
    setTimeout(function () {
        $('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();
    }, 33000 + j*51000 );
    setTimeout(function () {
        $('#div_y2015').click();
    }, 36000+ j*51000  );
    setTimeout(function () {
        $('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();
    }, 39000  + j*51000);
    setTimeout(function () {
        $('#div_y2016').click();
    }, 42000+ j*51000  );
    setTimeout(function () {
        $('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();
    }, 45000 + j*51000 );
    setTimeout(function () {
        $('#div_y2017').click();
    }, 48000 + j*51000 );
    setTimeout(function () {
        $('#viewCurrentRegionData_dd_area > div > div.combineGrid > a').click();
    }, 51000 + j*51000 );
})
```

## Data Order (by time): 5 for each area.
| Data attribute | Filename |
| --- | --- |
| Population 2000 Gaepo | data_view.xls |
| Population 2005 Gaepo | ... |
| Population 2010 Gaepo | ... |
| Population 2015 Gaepo | ... |
| Population 2016 Gaepo | ... |
| Population 2017 Gaepo | data_view (5).xls |
