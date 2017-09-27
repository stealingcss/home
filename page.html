<!DOCTYPE html>
<!--

    Author:        Twily                                        2015
    Website:       http://twily.info/
    Compatibility: Mozilla Firefox, Google Chrome
                   (For the slideshow to work this file cannot be run from a web server)

    Search Usage:  "artist!i" will find images for "artist"

-->
<html>
<head>
<meta http-equiv="Content-Type" content="text/html;charset=UTF-8" />
<title>New Tab</title>

<style type="text/css">
/*
    >> Search and Replace to change color scheme

    * (If you make two or more the same value you will need to
       manually separate the colors in the code later to undo) 

    #17181A - Background        #D54A56 - Color Mnu1
    #323232 - Content BG        #84BD3F - Color Mnu2
    #AAABAD - Content FG        #D753A4 - Color Mnu3
    #CECFD1 - C FG Light        #6F67E6 - Color Mnu4
    #111113 - L FG Hover

    Transition: "transition: .2s ease-out"
    Menu Width: "width: 200px"
    Margin Top: "margin-top: -75px"
    Border Rad: "border-radius: 1px"
*/

html,body {
    margin: 0; padding: 0; overflow: hidden;
    width: 100%; height: 100%;
    font-family: "Droid Sans", "Liberation Sans", "DejaVu Sans", "Segoe UI", Sans; font-size: 10pt;
    background: #232323;
}
*:focus  { outline: none; }
ul, li   { list-style-type: none; margin: 0; padding: 0; }
textarea { background: transparent; color: #CECFD1; }

a, a:link, a:visited { color: #CECFD1; text-decoration: none; transition: .2s ease-out; }
a:hover, a:active    { color: #111113; }



#center { position: relative; width: 100%; height: 100%; }
#center #content {
    margin: 0; overflow: visible; width: 100%; height: auto;
    position: absolute; top: 50%; transform: translate(0,-50%);
    text-align: center; opacity: 1; z-index: 10; background: #232323; /* #232323 || transparent */
}

#q {
    width: calc((200px * 4) - (8px * 2));
    background: #323232; color: #CECFD1;
    border: 0; border-radius: 1px;
    font-family: "Droid Sans", "Liberation Sans", "DejaVu Sans", "Segoe UI", Sans; font-size: 12pt;
    padding: 4px 8px; height: 24px;
}

#more {
    background: transparent; color: #AAABAD; display: block; 
    text-align: center; margin: 0 auto; width: 32px; height: 32px;
    font-weight: bold; cursor: default;
}
    #plus {
        border: 0; border-radius: 1px 1px 0 0; width: 32px; height: 32px; font-size: 12pt;
        background: transparent; color: #CECFD1; font-weight: bold; cursor: pointer;
        transition: .2s ease-out;
    }
    #help {
        display: block; visibility: hidden; width: 320px; cursor: default;
        position: absolute; left: 0; right: 0; margin: auto;
        font-family: "PragmataPro", "Droid Sans Mono", "Liberation Sans Mono", "DejaVu Sans Mono", "Consolas", "Lucida Console", monospace;
        padding: 8px; text-align: left; border-radius: 1px; opacity: 0;
        background: #323232; color: #AAABAD; transition: .2s ease-out;
    }
    #more:hover #plus { background: #323232; }
    #more:hover #help { visibility: visible; opacity: 1; }
        #note { width: 100%; height: 100px; resize: none; border: 0; outline: 0; }

#menu {
    width: 100%; height: 32px; margin: 0 auto;
    background: transparent; color: #AAABAD; cursor: default;
}
    #mnu                   { height: 32px; line-height: 32px; width: calc((200px * 4) + 1px); }

    #menu ul               { display: inline-table; position: relative; list-style: none; }
    #menu label            { padding: 0; display: inline-block; font-weight: bold; width: 200px; /* menu width */ }

    #menu ul li            { float: left; border-radius: 0 0 1px 1px; height: 32px; text-align: center; transition: .2s ease-out; }
    #menu ul li:hover      { background: #323232; color: #cecfd1;  }
    #menu ul li a          { display: block; white-space: nowrap; padding: 0 10px; }

    #menu ul ul {
        display: flex; flex-flow: column wrap; /* column | row(-reverse) */ align-content: flex-start;
        visibility: hidden; opacity: 0; width: calc(200px * 4); /* cols */ height: calc(32px * 3); /* rows */
        position: absolute; bottom: 100%; left: 0; z-index: 11;
        background: #323232; border-radius: 1px; transition: .2s ease-out;
    }
    #menu ul li:hover > ul { bottom: 100%; visibility: visible; opacity: 1; z-index: 12; height: calc(32px * 3); /* rows */ }
    #menu ul ul li { background: #323232; border-radius: 1px; height: 32px; text-align: left; width: 200px; /* menu width */ }

    /* Menu Colors */
    #menu ul #mnu_1 li:hover { background: #D54A56; }
    #menu ul #mnu_2 li:hover { background: #84BD3F; }
    #menu ul #mnu_3 li:hover { background: #D753A4; }
    #menu ul #mnu_4 li:hover { background: #6F67E6; }

    #menu img { position: relative; top: 3px; left: -3px; width: 16px; height: 16px; visibility: hidden; }
</style>
<script type="text/javascript" language="javascript">
var $=function(id) { return document.getElementById(id); };

var help="<ul> \
    <li><b>!g</b> = Search Google (Default)</li> \
    <li><b>!i</b> = Search Google Images</li> \
    <li><b>!m</b> = Search IMDb</li> \
    <li><b>!u</b> = Search Urban Dictionary</li> \
    <li><b>!w</b> = Search Wikipedia</li> \
    <li><b>!y</b> = Search YouTube</li> \
</ul>";

var search=[ // Search engines
    ["",    "https://www.google.com/#q="],                           // Google (Default)
    ["!g",  "https://www.google.com/#q="],                           // Google
    ["!i",  "https://www.google.com/search?tbm=isch&q="],            // Google Images
    ["!t",  "https://rarbg.to/torrents.php?search="],                         // rarbg
    ["!u",  "http://www.urbandictionary.com/define.php?term="],     // Urban Dictionary
    ["!w",  "http://en.wikipedia.org/w/index.php?search="],         // Wikipedia
    ["!y",  "https://www.youtube.com/results?search_query="],       // YouTube
];

var menu=[ // Menu titles
    "CHANGE",                                                        // mnu_1
    "questions",                                                        // mnu_2
    "dab",                                                        // mnu_3
    "mnu_4",                                                        // mnu_4
];

var showFavicon = true;                                             // Enable/Disable Link Favicons (img)

// Link setup (separate with ["", "", ""],)
// Format: ["Name", "URL", "Custom Favicon"],
var links=[
    // Links -           mnu_1
    ["YouTube",                      "https://www.youtube.com/feed/subscriptions",                 ""],
    ["userstyles",                       "https://userstyles.org/",                  ""],
    ["anime",                           "http://www.masterani.me/",                      ""],
    ["filelist",                        "http://filelist.ro/",                   ""],
    ["freakz",                             "https://wow.freakz.ro/",                       ""],
    ["twitch",                       "http://www.twitch.tv/directory/following",                   ""],
    ["reddit",                             "https://www.reddit.com/",                        ""],
    ["twitter",                              "https://twitter.com/",                         ""],
    ["imgur",                       "https://imgur.com/",                  ""],
    ["actions",                        "https://www.playerauctions.com/",                   ""],
    ["rarbg",                    "https://rarbg.to/torrents.php",              ""],
    ["Steam",                              "http://store.steampowered.com/",                         ""],

    ["", "", ""],

    // 4chan -          mnu_2
    ["/b/ - Random",                    "https://boards.4chan.org/b/",   ""],
    ["/a/ - Anime",                     "https://boards.4chan.org/a/",   ""],
    ["/v/ - Video Games",                     "https://boards.4chan.org/v/",          ""],
    ["/vg/ - vydra Generals",                "https://boards.4chan.org/vg/",   "http://s.4cdn.org/image/favicon-ws.ico"],
    ["/g/ - Technology",               "https://boards.4chan.org/g/", ""],
    ["/w/ - Anime Wallpapers",                    "https://boards.4chan.org/w/",   ""],
    ["/pol/ - Politically Incorrect",   "https://boards.4chan.org/pol/", ""],
    ["/wg/ - Wallpaper General",        "https://boards.4chan.org/wg/",  ""],
	["/wsg/ - Worksafe GIF",        "https://boards.4chan.org/wsg/",  ""],

    ["", "", ""],

    // music -  mnu_3
    ["spotify",                      "https://play.spotify.com/browse",              ""],
    ["youtube liked",                      "https://www.youtube.com/playlist?list=LLbQ5m88bN-WP6YmaP8jkpEQ",               ""],
    ["vintage",                      "https://www.stereodose.com/user_playlist/26895/vintage-news",           "https://i.imgur.com/Eq6j0MG.png"],
    ["BRNA",                           "http://hypster.com/hypsterPlayer/MPL?media_type=playlist&playlist_id=6739915&us_id=5042900",                   ""],
    ["dnb",                           "https://drumandbass.fm/",                   "https://i.imgur.com/yCxchVN.png"],
	["lobby",                           "https://www.dubtrack.fm/",                   ""],
	["dubbase",                           "http://dubbase.fm/",                   ""],
	["radio ro",                           "http://asculta.fm/",                   "https://i.imgur.com/PXFBEbH.png"],
    ["MLGslayer",                           "https://www.deezer.com/playlist/1226777521",                   ""],
	["trap.fm",                           "http://trap.fm/",                   ""],
	["contemplation",                           "https://www.stereodose.com/user_playlist/26483/contemplation",                   ""],
	["demo",                           "https://soundcloud.com/demolition_d",                   ""],
	["", "", ""],

    // Other -          mnu_4
    ["zippy",                          "http://zippysharesearch.com/",               ""],
    ["horriblesubs",                        "http://horriblesubs.info/",                 ""],
    ["gmail",                             "https://mail.google.com/mail/u/0/#inbox",                ""],
    ["yahoo mail",                         "https://us-mg5.mail.yahoo.com/neo/launch?",              ""],
    ["rip nyaa",                        "https://nyaa.si/",                  ""],
    ["hotmail",                         "http://outlook.com",                   ""],
    ["one drive",                        "https://onedrive.live.com/",    ""],
    ["tuta",                          "https://app.tutanota.com/#box",               ""],
    ["upload",                         "https://safe.moe/",                    ""],
    ["image bot",                      "https://nik.bot.nu/",               ""],
    ["iqdb",                         "https://iqdb.org/",                   ""],
    ["Wallhaven",                       "http://alpha.wallhaven.cc",            ""],
];

// Command to generate imagelist (GNU/Linux) [Requires find, sed and vim]
// $ function list() { echo "var filepath=\"file://"$(pwd)"/\";" && find "$1" -maxdepth 1 -type f -regex ".*\.\(jpg\|jpeg\|png\)" -exec echo "    "\"{}\", \; | sed "s/%/%25/g" | sed "s/\.\///g" | vim -; }; list .
// 
// If filenames (or the path) contain '%' they will need to be replaced by '%25' (Eg.: ..%25.. to ..%2525..)
// (The command above does this automatically using sed)
var imagelist=[
    "wallhaven-110491.jpg",
    "wallhaven-123187.jpg",
    "wallhaven-134400.jpg",
    "wallhaven-137115.jpg",
    "wallhaven-149753.jpg",
    "wallhaven-20260.jpg",
    "wallhaven-26620.jpg",
    "wallhaven-31652.jpg",
    "wallhaven-50083.jpg",
    "wallhaven-51234.jpg",
    "wallhaven-54308.jpg",
    "wallhaven-6463.jpg",
    "wallhaven-65157.jpg",
    "wallhaven-6688.jpg",
    "wallhaven-69760.jpg",
    "wallhaven-72147.jpg",
    "wallhaven-82896.jpg",
    "wallhaven-8489.jpg",
    "wallhaven-86566.jpg",
];

var wTimer=5;                                                                   // Seconds before next image
var wOpacity=25;                                                                // 0 (Transparent) - 100 (Opaque)
var filepath="D:\stuff\shit\desktop";               // Path to find images (filepath+imagelist[x])

var i,ss="";
function init() {
    for(i=0;i<search.length;i++) if(search[i][0]=="") ss=search[i][1];
    if(ss=="") alert("Error: Missing default search engine!");

    $('help').innerHTML=help;
    if(localStorage.getItem('note')!=null) if(localStorage.getItem('note').length!=0) toggleNote();
    build();

    nextImage();                                                                // Show first image
    if(imagelist.length>1) setInterval("nextImage();",wTimer*1000);             // Run the slideshow
    $('q').value="";
    $('q').focus();
}

var wshow="img1",whide="img2",newimg,curimg;
function nextImage() {
    curimg=newimg;
    while(newimg==curimg) newimg=Math.floor(Math.random()*imagelist.length);    // Generate next random image
    (new Image()).src=filepath+imagelist[newimg];                               // Preload next image

    whide=[wshow,wshow=whide][0];                                               // Swap values
    $(wshow).style.backgroundImage="url('"+filepath+imagelist[curimg]+"')";     // Show current image
    $(wshow).style.opacity=wOpacity/100;
    $(whide).style.opacity=0;

    if(curimg==null) nextImage();                                               // Buffer one image ahead
}

function build() { // Build menu
    $('mnu').innerHTML="";

    for(i=0;i<menu.length;i++) { // Menu titles
        $('mnu').innerHTML+="<li><label>"+menu[i]+"</label>\n<ul id=\"mnu_"+(i+1)+"\"></ul></li>";
    }

    var m=1,skip=false;
    for(i=0;i<links.length;i++) { // Menu links
        if(links[i][0]=="" && links[i][1]=="") skip=true;

        if(!skip) {
            var printimg="";

            if(showFavicon) {
                var favicon;
                if(links[i][2]!="") favicon=links[i][2];
                else                favicon=getFavicon(links[i][1]);

                printimg="<img id=\"img_"+i+"\" src=\""+favicon+"\""+" onload=\"javascript:this.style.visibility='inherit';\" /> ";
            }

            $('mnu_'+m).innerHTML+="<li><a href=\""+links[i][1]+"\" target=\"_self\">"+printimg+links[i][0]+"</a></li>";
        } else {
            skip=false; m++;
        }
    }
}

/*
    Optional patch for using "!i" before the search query: http://pastebin.com/Lw24tQ81
*/
function handleQuery(e,q) { // Handle search query
    var key=e.keyCode || e.which;

    if(key==13) { // Enter
        var x=q.lastIndexOf("!");

        if(x!=-1 && x>=q.length-2) {
            for(i=0;i<search.length;i++) {
                if(search[i][0]==q.substr(x)) { // Find "*!i"
                    window.location=search[i][1]+q.substr(0,x).replace(/&/g,"%26");
                    return true;
                }
            }
            // Invalid "!i", use default
            window.location=ss+q.substr(0,x).replace(/&/g,"%26");
        } else {
            // "!i" where not specified, use default
            window.location=ss+q.replace(/&/g,"%26");
        }
    }
}

function getFavicon(url) {
    var l=document.createElement("a");
    l.href=url;

    return l.protocol+"//"+l.hostname+"/favicon.ico";
}

function toggleNote() {
    if($('note')==null) {
        $('help').innerHTML="<textarea id='note' spellcheck='false' placeholder='Store temporary note...'></textarea>";
        if(localStorage.getItem('note')!=null) $('note').value=localStorage.getItem('note');
        $('note').addEventListener('change',function() { localStorage.setItem('note',$('note').value); });
        $('plus').value="-";
        $('note').focus();
    } else {
        $('help').innerHTML=help;
        $('plus').value="+";
        $('q').focus();
    }
}
</script>
</head>
<body onload="javascript:init();">

<div id="img1" class="slideshow"></div>
<div id="img2" class="slideshow"></div>

<div id="center">
    <div id="content">
        <div id="menu">
            <ul id="mnu"></ul>
        </div>
        <br />
        <input type="text" id="q" value="" placeholder="Search..." onkeypress="javascript:handleQuery(event,this.value);" onfocus="this.value=this.value" />
        <br /><br />
        <div id="more">
            <input type="button" id="plus" value="+" onclick="javascript:toggleNote();" />
            <br />
            <div id="help"></div>
        </div>
    </div>
</div>

</body>
</html>

