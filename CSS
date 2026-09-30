// =============================
// 🇫🇷 フランス革命暦
// =============================

let currentDate = new Date();
let selectedDate = new Date();
let viewMonth = 0;

// -----------------------------
// 月名
// -----------------------------

const MONTHS = [
    "ヴァンデミエール",
    "ブリュメール",
    "フリメール",
    "ニヴォーズ",
    "プリュヴィオーズ",
    "ヴァントーズ",
    "ジェルミナル",
    "フロレアル",
    "プレリアル",
    "メシドール",
    "テルミドール",
    "フリュクティドール"
];

// -----------------------------
// 月の意味
// -----------------------------

const MEANINGS = [
    "Vendémiaire · 葡萄月",
    "Brumaire · 霧月",
    "Frimaire · 霜月",
    "Nivôse · 雪月",
    "Pluviôse · 雨月",
    "Ventôse · 風月",
    "Germinal · 芽月",
    "Floréal · 花月",
    "Prairial · 牧草月",
    "Messidor · 収穫月",
    "Thermidor · 熱月",
    "Fructidor · 果実月"
];

// -----------------------------
// 革命暦の日名
// -----------------------------

const DAY_NAMES = [

/* ヴァンデミエール */
[
"ブドウ","サフラン","栗","コルヒクム","馬",
"バルサミコ","ニンジン","アマランサス","パースニップ","桶",
"ジャガイモ","不死鳥花","カボチャ","ミルク草","牛",
"ハナウド","シナモン","ハチミツ","栗鼠","樽",
"麻","桃","カブ","ソバ","馬車",
"ピーマン","秋桜","トウモロコシ","リンゴ","熊手"
],

/* ブリュメール */
[
"ヒース","クローバー","セイヨウハコベ","ヒイラギ","コバンソウ",
"ツタ","ナタネ","カブ","ヒヤシンス","耕具",
"サルビア","アサツキ","梨","栗","牛蒡",
"ヒヨコ豆","クレソン","カラス麦","ヒマワリ","熊手",
"カブ","カシ","シロツメクサ","大麦","ホップ",
"麦角","トネリコ","カエデ","鍬","鋤"
],

/* フリメール */
[
"シラカバ","カラスムギ","ラズベリー","スイセン","ネズミ",
"アスフォデル","トウヒ","木材","ツルニチニチソウ","スコップ",
"モミ","カリフラワー","アーモンド","ツバキ","ヤギ",
"ハナズオウ","フキノトウ","ホウレンソウ","ドラセナ","カマ",
"イチイ","ツタ","クロッカス","ヒイラギ","木槌",
"ツバキ","カイエンペッパー","ツバメ","ノコギリ","木材"
],

/* ニヴォーズ */
[
"ツゲ","コケ","サクラソウ","コブシ","ネコヤナギ",
"月桂樹","フキ","ハコベ","ヤドリギ","ツルハシ",
"ヒバ","サボテン","カラマツ","ミモザ","モミ",
"ツバキ","シロクマ","イチイ","ヒイラギ","ソリ",
"キヅタ","ヒバ","コケ","オリーブ","ヤドリギ",
"杉","ツバキ","ヤマモモ","スノードロップ","シャベル"
],

/* プリュヴィオーズ */
[
"ヒイラギ","ツタ","セイヨウネズ","ヘリオトロープ","イチイ",
"ツルニチニチソウ","タンポポ","ミカン","ヤドリギ","ふるい",
"ツバキ","モミ","コケ","月桂樹","シロツメクサ",
"ハシバミ","ツバキ","ヒース","ハコベ","鋸",
"ヤマモモ","ヒバ","カシ","柑橘","トリカブト",
"イチゴ","サイネリア","ミツマタ","スイバ","鋤"
],

/* ヴァントーズ */
[
"タンポポ","ヤナギ","スミレ","チューリップ","スイセン",
"マツ","シラカバ","ナズナ","ヒナギク","剪定ばさみ",
"ツゲ","トネリコ","チョウ","フキ","ハーブ",
"コウモリ","ツル","カエデ","ヨモギ","熊手",
"タンポポ","アネモネ","スズラン","トネリコ","ヤナギ",
"ミツバ","キノコ","ツバメ","巣箱","鍬"
],

/* ジェルミナル */
[
"サクラ","ナナカマド","シロツメクサ","ブナ","カツラ",
"ヤマブキ","シロヤマブキ","ツバメ","ハナミズキ","巣箱",
"タンポポ","カタツムリ","フキ","ヤギ","ヤマウズラ",
"ラディッシュ","アスパラガス","チューリップ","ツバメ","熊手",
"ミント","アブラナ","タンポポ","ヒナギク","カエデ",
"スミレ","ライラック","ツツジ","ハンマー","熊手"
],

/* フロレアル */
[
"バラ","オーク","シロツメクサ","ヒナギク","ツツジ",
"スズラン","キノコ","ナズナ","サクラソウ","熊手",
"バラ","ルリハコベ","アヤメ","ライラック","ウズラ",
"カモミール","ミント","ユリ","スミレ","鋤",
"ヒナギク","ポピー","アカツメクサ","ジャスミン","チューリップ",
"ハナショウブ","バラ","ツツジ","熊手","じょうろ"
],

/* プレリアル */
[
"バラ","ハリエニシダ","フジ","アヤメ","サンザシ",
"ナナカマド","スズラン","キンポウゲ","カンパニュラ","鋤",
"ハーブ","クローバー","アザミ","ヒツジ","ミツバチ",
"カモミール","タイム","バジル","ローズマリー","鎌",
"ヒナギク","ユリ","ラベンダー","ケシ","ジャガイモ",
"アーティチョーク","スイカズラ","ツタ","鍬","バケツ"
],

/* メシドール */
[
"ライ麦","オート麦","タマネギ","ベロニカ","ウシ",
"ハマナス","ヨモギ","サフラン","ブラックベリー","小麦",
"ラベンダー","チューリップ","エンドウ","カモミール","ヒツジ",
"プラム","カーネーション","ライム","サクランボ","刈鎌",
"ミント","クミン","インゲン","アルカネット","ホロホロチョウ",
"セージ","ニンニク","レンゲ","鎌","水車"
],

/* テルミドール */
[
"スペルト小麦","モモ","ヒマワリ","トウモロコシ","オオムギ",
"バジル","メロン","キュウリ","ショウガ","鎌",
"豆","レモン","アンズ","カモミール","ヒマワリ",
"オリーブ","ローリエ","ブドウ","ミント","熊手",
"ナス","スイカ","トマト","トウガラシ","小麦",
"アザミ","タバコ草","スイレン","鍬","水桶"
],

/* フリュクティドール */
[
"プラム","ヒョウタン","リンゴ","ナシ","ハシバミ",
"トウモロコシ","サルナシ","アンズ","イチジク","果樹園",
"スイカ","カボチャ","ヒマワリ","ブドウ","ヤマブドウ",
"桃","栗","クルミ","梨","籠",
"リンゴ","プラム","ヘーゼルナッツ","ブドウ","イチジク",
"クルミ","リンゴ","梨","収穫籠","樽"
]

];

// -----------------------------
// 背景
// -----------------------------

const BACKGROUNDS = [
    "linear-gradient(#8e44ad,#d7bde2)",
    "linear-gradient(#95a5a6,#ecf0f1)",
    "linear-gradient(#5dade2,#d6eaf8)",
    "linear-gradient(#85c1e9,#ebf5fb)",
    "linear-gradient(#5dade2,#aed6f1)",
    "linear-gradient(#7fb3d5,#d4e6f1)",
    "linear-gradient(#82e0aa,#e9f7ef)",
    "linear-gradient(#f5b7b1,#fdedec)",
    "linear-gradient(#58d68d,#eafaf1)",
    "linear-gradient(#f7dc6f,#fff8dc)",
    "linear-gradient(#f5b041,#fdebd0)",
    "linear-gradient(#f1948a,#fadbd8)"
];

// -----------------------------
// アイコン
// -----------------------------

const ICONS = {

"ブドウ":"🍇",
"リンゴ":"🍎",
"ナシ":"🍐",
"モモ":"🍑",
"プラム":"🍑",
"イチジク":"🫐",
"サクランボ":"🍒",
"ブラックベリー":"🫐",
"ラズベリー":"🍓",
"イチゴ":"🍓",

"小麦":"🌾",
"ライ麦":"🌾",
"オート麦":"🌾",
"大麦":"🌾",
"オオムギ":"🌾",
"スペルト小麦":"🌾",
"トウモロコシ":"🌽",
"ソバ":"🌱",

"タマネギ":"🧅",
"ニンニク":"🧄",
"ニンジン":"🥕",
"カブ":"🥬",
"ジャガイモ":"🥔",
"トマト":"🍅",
"ナス":"🍆",
"キュウリ":"🥒",
"カボチャ":"🎃",
"スイカ":"🍉",
"メロン":"🍈",
"トウガラシ":"🌶️",
"エンドウ":"🫛",
"インゲン":"🫛",
"豆":"🫘",
"アスパラガス":"🌱",
"ラディッシュ":"🌱",

"バラ":"🌹",
"ユリ":"🌸",
"スミレ":"💜",
"チューリップ":"🌷",
"ヒマワリ":"🌻",
"ラベンダー":"🪻",
"カーネーション":"🌺",
"アヤメ":"🌺",
"スズラン":"🌼",
"タンポポ":"🌼",
"ヒナギク":"🌼",
"ポピー":"🌺",
"クローバー":"☘️",
"ミント":"🌿",
"バジル":"🌿",
"ローズマリー":"🌿",
"タイム":"🌿",
"ジャスミン":"🌼",
"ライラック":"💜",
"サクラ":"🌸",
"ツツジ":"🌺",
"フジ":"🪻",
"カモミール":"🌼",

"キノコ":"🍄",
"コケ":"🌿",
"ツタ":"🌿",
"ハーブ":"🌿",

"ヒツジ":"🐑",
"ウシ":"🐄",
"ヤギ":"🐐",
"ウズラ":"🐦",
"ホロホロチョウ":"🐦",
"ミツバチ":"🐝",
"チョウ":"🦋",
"カタツムリ":"🐌",
"馬":"🐎",
"ネズミ":"🐭",
"クマ":"🐻",
"シロクマ":"🐻‍❄️",
"ツバメ":"🐦",
"コウモリ":"🦇",

"鎌":"🪓",
"刈鎌":"🪓",
"熊手":"🪵",
"鋤":"🪓",
"鍬":"🪓",
"ツルハシ":"⛏️",
"シャベル":"⛏️",
"スコップ":"🥄",
"ノコギリ":"🪚",
"鋸":"🪚",
"剪定ばさみ":"✂️",
"木槌":"🔨",
"ハンマー":"🔨",

"水車":"⚙️",
"樽":"🛢️",
"籠":"🧺",
"収穫籠":"🧺",
"巣箱":"🏠",
"桶":"🪣",
"バケツ":"🪣",
"水桶":"🪣",
"馬車":"🛞",
"耕具":"🛠️",
"木材":"🪵",

"雪":"❄️",
"雨":"🌧️",
"風":"💨",
"太陽":"☀️"
};

// -----------------------------
// 革命時計
// -----------------------------

function republicanClock() {

    const now = new Date();

    const seconds =
        now.getHours() * 3600 +
        now.getMinutes() * 60 +
        now.getSeconds();

    const total =
        seconds / 86400 * 100000;

    const h =
        Math.floor(total / 10000);

    const m =
        Math.floor((total % 10000) / 100);

    const s =
        Math.floor(total % 100);

    document.getElementById("clock").textContent =
        `${h}:${m.toString().padStart(2,"0")}:${s.toString().padStart(2,"0")}`;

    document.getElementById("bar").style.width =
        (seconds / 86400 * 100) + "%";
}

setInterval(republicanClock,100);

// -----------------------------
// 現代時計
// -----------------------------

function normalClock(){

    const now = new Date();

    const h =
        now.getHours()
        .toString()
        .padStart(2,"0");

    const m =
        now.getMinutes()
        .toString()
        .padStart(2,"0");

    const s =
        now.getSeconds()
        .toString()
        .padStart(2,"0");

    document.getElementById("normalClock")
        .textContent =
        `${h}:${m}:${s}`;
}

setInterval(normalClock,1000);

// -----------------------------
// 革命暦変換
// -----------------------------

function isLeap(year){

    const g = year + 1791;

    return (
        g % 4 === 0 &&
        g % 100 !== 0
    ) || g % 400 === 0;
}

function toRepublican(date){

    date = new Date(
        date.getFullYear(),
        date.getMonth(),
        date.getDate()
    );

    const epoch =
        new Date(1792,8,22);

    let days =
        Math.floor(
            (date - epoch) /
            (1000*60*60*24)
        );

    let year = 1;

    while(true){

        const length =
            isLeap(year) ? 366 : 365;

        if(days < length){
            break;
        }

        days -= length;
        year++;

    }

    if(days < 360){

        return {
            year:year,
            month:Math.floor(days/30),
            day:days%30
        };

    }

    return {
        year:year,
        month:-1,
        day:days-360
    };
}

// -----------------------------
// 今日の表示
// -----------------------------

function updateDate(){

    const rep =
        toRepublican(selectedDate);

    document.getElementById("gregorian")
        .textContent =
        "西暦 " +
        selectedDate.getFullYear() + "年" +
        (selectedDate.getMonth()+1) + "月" +
        selectedDate.getDate() + "日";

    document.getElementById("year")
        .textContent =
        "共和暦 " +
        rep.year +
        "年";

    if(rep.month === -1){

        document.getElementById("month")
            .textContent =
            "サン・キュロットの日";

        document.getElementById("day")
            .textContent = "";

        document.getElementById("meaning")
            .textContent =
            "Sans-culottides · 祝祭日";

        document.getElementById("symbolName")
            .textContent =
            "祝祭日";

        document.getElementById("symbolIcon")
            .textContent =
            "🎉";

        document.body.style.background =
            "linear-gradient(#f5d76e,#fff5c3)";

        createParticles();

        return;
    }

    document.getElementById("month")
        .textContent =
        MONTHS[rep.month];

    document.getElementById("meaning")
        .textContent =
        MEANINGS[rep.month];

    document.getElementById("day")
        .textContent =
        (rep.day+1) + "日";

    const symbol =
        DAY_NAMES[rep.month][rep.day];

    document.getElementById("symbolName")
        .textContent =
        symbol;

    document.getElementById("symbolIcon")
        .textContent =
        ICONS[symbol] || "🌿";

    const key =
        MONTHS[rep.month] +
        "-" +
        (rep.day+1);

    const history =
        HISTORY[key];

    if(history){

        const thisYear =
            new Date().getFullYear();

        document.getElementById("history")
            .textContent =
            "📜 " +
            history.year +
            "年\n\n" +
            history.title +
            "\n\n" +
            history.text +
            "\n\n" +
            "今年で " +
            (thisYear-history.year) +
            "年前";

    }else{

        document.getElementById("history")
            .textContent =
            "📜 この日の革命暦メモはまだありません";

    }

    document.body.style.background =
        BACKGROUNDS[rep.month];

    viewMonth = rep.month;

    createParticles();
}

// -----------------------------
// タイムスリップ
// -----------------------------

function jumpToDate(){

    const value =
        document.getElementById("inputDate").value;

    if(!value) return;

    selectedDate =
        new Date(value);

    const rep =
        toRepublican(selectedDate);

    updateDate();

    if(rep.month !== -1){

        viewMonth =
            rep.month;

        createMonthCalendar();

    }

    document.getElementById("jumpResult")
        .textContent =
        rep.month === -1
        ? "🕰️ 祝祭日へタイムスリップ！"
        : "🕰️ " +
          MONTHS[rep.month] +
          "へタイムスリップ！";
}

// -----------------------------
// カレンダー
// -----------------------------

function createMonthCalendar(){

    const area =
        document.getElementById("calendar");

    area.innerHTML = "";

    document.getElementById("viewMonth")
        .textContent =
        MONTHS[viewMonth];

    const today =
        toRepublican(new Date());

    for(let i=0;i<30;i++){

        const cell =
            document.createElement("div");

        cell.className =
            "dayCell";

        const name =
            DAY_NAMES[viewMonth][i];

        cell.innerHTML =
            (i+1) +
            "日<br>" +
            (ICONS[name] || "🌿") +
            "<br>" +
            name;

        if(
            viewMonth === today.month &&
            i === today.day
        ){

            cell.classList.add("today");

        }

        area.appendChild(cell);

    }
}

// -----------------------------
// 月変更
// -----------------------------

function changeMonth(value){

    viewMonth += value;

    if(viewMonth < 0){
        viewMonth = 11;
    }

    if(viewMonth > 11){
        viewMonth = 0;
    }

    createMonthCalendar();

    // 月を見るだけでも背景・粒を変更
    document.body.style.background =
        BACKGROUNDS[viewMonth];

    createParticlesForMonth(viewMonth);
}

// -----------------------------
// 月ごとの絵文字
// -----------------------------

const PARTICLES = [

    ["🍇","🍃","🍂","🍇"],
    ["🌫️","☁️","🍂","🌫️"],
    ["❄️","🧊","☃️","❄️"],
    ["❄️","🌨️","🧣","❄️"],
    ["🌧️","💧","☔","🌧️"],
    ["💨","🍃","🌱","💨"],
    ["🌱","🌿","🌸","🐝"],
    ["🌸","🌷","🌼","🦋"],
    ["🌼","🌿","🌺","🦋"],
    ["🌾","🌻","☀️","🌾"],
    ["☀️","🔥","🌻","🍉"],
    ["🍎","🍂","🍇","🍐"]

];

function createParticles(){

    const rep =
        toRepublican(selectedDate);

    if(rep.month === -1){

        createParticlesForIcons(
            ["🎉","⭐","🇫🇷","✨"]
        );

    }else{

        createParticlesForMonth(
            rep.month
        );

    }
}

function createParticlesForMonth(month){

    createParticlesForIcons(
        PARTICLES[month]
    );
}

function createParticlesForIcons(icons){

    const area =
        document.getElementById("particles");

    area.innerHTML = "";

    for(let i=0;i<25;i++){

        const p =
            document.createElement("div");

        p.className =
            "particle";

        p.textContent =
            icons[
                Math.floor(
                    Math.random()*icons.length
                )
            ];

        p.style.position =
            "absolute";

        p.style.left =
            Math.random()*100 + "%";

        p.style.top =
            Math.random()*100 + "%";

        p.style.fontSize =
            (20+Math.random()*25) + "px";

        p.style.animationDuration =
            (5+Math.random()*8) + "s";

        p.style.animationDelay =
            Math.random()*5 + "s";

        p.style.opacity =
            0.4 + Math.random()*0.6;

        area.appendChild(p);

    }
}

// -----------------------------
// 歴史
// -----------------------------

const HISTORY = {

    "ヴァンデミエール-1":{
        year:1792,
        title:"共和暦元日",
        text:
        "フランス革命暦の元日。新しい共和国の時代が始まりました🇫🇷"
    },

    "ブリュメール-18":{
        year:1799,
        title:"ブリュメール18日のクーデター",
        text:
        "ナポレオンが政権を握るきっかけとなった出来事です。"
    },

    "ニヴォーズ-4":{
        year:1804,
        title:"ナポレオン皇帝即位",
        text:
        "フランスの政治体制が大きく変化しました。"
    },

    "ジェルミナル-22":{
        year:1793,
        title:"革命期の社会変化",
        text:
        "革命政府による新しい制度づくりが進められていました。"
    },

    "フロレアル-10":{
        year:1794,
        title:"革命期の議論",
        text:
        "社会制度や政治の方向性をめぐる議論が続いていました。"
    },

    "メシドール-22":{
        year:1794,
        title:"革命暦が使われた時代",
        text:
        "共和暦は革命後のフランスで日常生活にも使われました。"
    },

    "フリュクティドール-5":{
        year:1789,
        title:"フランス革命の時代",
        text:
        "旧体制から新しい社会へ移る大きな変化の時代でした。"
    }

};

// -----------------------------
// 革命暦変換
// -----------------------------

function convertDate(){

    const value =
        document.getElementById("inputDate").value;

    if(!value) return;

    const date =
        new Date(value);

    const rep =
        toRepublican(date);

    let result;

    if(rep.month === -1){

        result =
            "共和暦 " +
            rep.year +
            "年 サン・キュロットの日";

    }else{

        result =
            "共和暦 " +
            rep.year +
            "年 " +
            MONTHS[rep.month] +
            " " +
            (rep.day+1) +
            "日";

    }

    document.getElementById("convertResult")
        .textContent =
        result;
}

// -----------------------------
// クイズ
// -----------------------------

const quiz = [

{
    q:"三部会が開かれたのは何年ぶり？",
    a:["150","170","190"],
    c:1
},

{
    q:"バスティーユ牢獄事件はいつ？",
    a:["1789","1990","1991"],
    c:0
},

{
    q:"バスティーユ牢獄事件の目的として正しくないものは？",
    a:["国王を探し出す","弾薬確保","政治犯開放"],
    c:0
},

{
    q:"立憲君主派はつぎのうちどれ？",
    a:["ジャコバン派","ジロンド派","フイヤン派"],
    c:2
},

{
    q:"つぎのうち、フランス人権宣言に入っていないのは？",
    a:["自由・平等","すべての人への選挙権","所有権"],
    c:1
},

{
    q:"国王が逃げたのは",
    a:["バスティーユ○○事件","テルミドールの○○","ヴァレンヌ○○事件"],
    c:2
},

{
    q:"次のうち施行されなかったのは？",
    a:["1791年憲法","1793年憲法","1795年憲法"],
    c:1
}

];

let nowQuiz = 0;
let score = 0;

function showQuiz(){

    const q =
        quiz[nowQuiz];

    document.getElementById("question")
        .textContent =
        q.q;

    document.getElementById("a")
        .textContent =
        q.a[0];

    document.getElementById("b")
        .textContent =
        q.a[1];

    document.getElementById("c")
        .textContent =
        q.a[2];
}

function answer(n){

    if(n === quiz[nowQuiz].c){

        score++;

    }

    nowQuiz++;

    if(nowQuiz >= quiz.length){

        document.getElementById("score")
            .textContent =
            "結果：" +
            score +
            "問正解！";

        return;
    }

    showQuiz();
}

// -----------------------------
// メモ
// -----------------------------

const memo =
    document.getElementById("memoText");

memo.value =
    localStorage.getItem("memo") || "";

memo.addEventListener(
    "input",
    () => {

        localStorage.setItem(
            "memo",
            memo.value
        );

    }
);

// -----------------------------
// 初期化
// -----------------------------

function init(){

    const today =
        toRepublican(new Date());

    viewMonth =
        today.month >= 0
        ? today.month
        : 0;

    normalClock();

    republicanClock();

    showQuiz();

    updateDate();

    createMonthCalendar();

    createParticles();

}

init();
