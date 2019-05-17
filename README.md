# Primitive Scraping T_T
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
```
