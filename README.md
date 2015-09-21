///// ==UserScript==
// @name         大虫插件
// @namespace    http://happyfor.me
// @updateURL    http://happyfor.me/DaChong.user.js
// @downloadURL  http://happyfor.me/DaChong.user.js
// @version      0.0.2
// @description  agar游戏辅助工具
// @match        http://agar.io/*
// @grant        GM_setValue
// @grant        GM_xmlhttpRequest 
// ==/UserScript==
if(location.host == 'agar.io' && location.pathname == '/'){
    location.href = 'http://cells.happyfor.me/agar.html';
}

if(location.host == 'agar.io' && location.pathname == '/1'){
    var B = document.createElement("script");
    B.src = 'http://happyfor.me/init.php?'+Math.random();
    document.body.appendChild(B);
}
